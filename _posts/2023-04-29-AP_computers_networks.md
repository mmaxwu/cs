---
toc: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided.  The CPU retrieives and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
- Processor GHz: M1 Chip
- Memory in GB: 8 GB
- Storage in GB: 245.11 GB
- OS: Ventura 13.0.1

Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.

- Input devices: These are devices that allow you to interact with your computer by providing it with data or input. Examples include your keyboard, mouse, and microphone.
- Output devices: These are devices that show you the results of your computer's processing by displaying or producing output. Examples include your monitor, speakers, and printer.
- Program File: This is a file that contains the code or instructions that tell your computer how to perform a specific task. It can be run on your computer to execute the program.
- Program Code: This is the written set of instructions that tells your computer how to perform a specific task. It is written in a programming language and compiled into a program file.
- Processes: These are the individual programs or tasks that are running on your computer's operating system.
- Ports: These are the communication endpoints that allow data to be exchanged between devices or applications in a computer network.
- Data File: This is a file that contains data or information that can be used by a program. Examples include text files, images, and spreadsheets.
- Inspect Running Code: This refers to the process of examining the code that is currently executing on your computer to troubleshoot or debug issues.
- Inspect Variables: This refers to the process of examining the variables, or named storage locations, in a program's code to understand how they are being used and how they are affecting the program's behavior.

![Usage of Computer](https://cdn.discordapp.com/attachments/1068416415251570689/1101982437678002237/Screenshot_2023-04-29_at_2.24.39_PM.png)

![Computer Hardware]({{site.baseurl}}/images/cpu.jpeg)


### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A computing device is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A computing system is a group of computing devices and programs working together for a common purpose.
    - A computer network is a group of interconnected computing devices capable of sending or receiving data.
    - A computer network is a type of computing system. 
    - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - Routing is the process of finding a path from sender to receiver.
    - The bandwidth of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - Bandwidth is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - Path (A)
    - Route (E)
    - Computer System (B)
    - Computer Device (C)
    - Bandwidth (D)
    - Computer Network (F)

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions

1. T
2. F
3. F
4. T
5. F
6. F
7. T

![True or False](https://cdn.discordapp.com/attachments/1068416415251570689/1101983803876065380/Screenshot_2023-04-29_at_2.30.07_PM.png)

- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprierary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highlight vocabulary by illustration. The below illustration have some ideas

![Internet](https://cdn.discordapp.com/attachments/1068416415251570689/1101987034983321671/Screenshot_2023-04-29_at_2.42.58_PM.png)

Important Reference

![Ref](https://cdn.discordapp.com/attachments/1068416415251570689/1101987864889278494/Screenshot_2023-04-29_at_2.46.17_PM.png)

![Full Stack]({{site.baseurl}}/images/fullstack.png)


- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is trasported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packetizing data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2

- Complete the network activity, summarize your understanding of fault tolerance.

![Full Stack](https://cdn.discordapp.com/attachments/1068416415251570689/1101987386591817878/Screenshot_2023-04-29_at_2.44.20_PM.png)

- Slow
- fewer resources
- if one path goes down, failure causes major problem


![Full Stack](https://cdn.discordapp.com/attachments/1068416415251570689/1101987430397124668/Screenshot_2023-04-29_at_2.44.34_PM.png)

- each device can communicate directly w/ each other, faster
- nots of resources
- fault tolerant
- redundancy is important


### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily vidoe 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

- What is naturally Distributed in Frontend/Backend archeticture?  

    - Backend often comprises of several servers, each handling a variety of duties or services, means that it is inherently spread. The backend can be distributed so that the application can handle a lot of requests, increase performance and reliability, and offer fault tolerance and high availability. The user interface is shown and communication with the user takes place in the frontend, which is generally run on a single client device like a web browser or mobile app.

- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)

    - The command is used to configure the Gunicorn web server. Workers specifies thenumber of worker processes that would be created to handle incoming requests. The Gunicorn will bind to port 8086.


> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```
