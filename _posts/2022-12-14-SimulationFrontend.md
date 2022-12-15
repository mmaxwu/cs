---
toc: true
layout: post
description: Unit 3.16 HW
title: Pendulum Simulation
categories: [Week 16, jupyter]
---

<!DOCTYPE html>
<html>
<head>
    <title>Pendulum Simulation</title>
</head>
<body>
    <canvas id="pendulum-canvas" width="500" height="500"></canvas>
    <script>
        // constants
        const GRAVITY = 9.81; // m/s^2
        const LENGTH = 200; // pixels
        const FRAME_RATE = 60; // frames per second
        const MASS = 10; // kg
        const DAMPING = 0.995; // unitless

        // state variables
        let theta = Math.PI / 4; // radians
        let omega = 0; // radians/second

        // canvas
        let canvas = document.getElementById('pendulum-canvas');
        let ctx = canvas.getContext('2d');

        // draw the pendulum
        function drawPendulum() {
            // calculate cartesian coordinates
            let x = LENGTH * Math.sin(theta);
            let y = LENGTH * Math.cos(theta);

            // clear canvas
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // draw the rope
            ctx.beginPath();
            ctx.moveTo(0, 0);
            ctx.lineTo(x, y);
            ctx.stroke();

            // draw the bob
            ctx.beginPath();
            ctx.arc(x, y, MASS, 0, 2 * Math.PI);
            ctx.fill();
        }

        // update the pendulum's state
        function updatePendulum() {
            // calculate acceleration
            let acceleration = (-GRAVITY / LENGTH) * Math.sin(theta);

            // update angular velocity
            omega += acceleration;

            // apply damping
            omega *= DAMPING;

            // update angle
            theta += omega;
        }

        // animation loop
        function animate() {
            // update pendulum
            updatePendulum();

            // draw pendulum
            drawPendulum();

            // request next frame
            requestAnimationFrame(animate);
        }

        // start animation
        animate();
    </script>
</body>
</html>
