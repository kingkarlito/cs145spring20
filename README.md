# CS 145, Spring 2020: Cloud Networking and Computing

## Overview

Clouds have become critical infrastructures for many applications in business and society (e.g., social media, public health, and entertainment). In this course, we will take a look inside the cloud infrastructure and learn critical technology trends and challenges in the networking and computing layers. We will discuss the design choices of performance, scalability, manageability, and cost in various cloud companies such as Amazon, Google, Microsoft, and Facebook. This course includes lectures and system programming projects.

- Instructor: Minlan Yu (MD 137)
- Lecture time: MW 1:30pm-2:45pm
- Location: TBD
- Office hour: M 12:30-1:30, MD 137
- Discussion list: [Piazza](https://piazza.com/class/jy80ngwm9123)
- Prerequisite: There are no official prerequisites. Recommended prep: system programming at the level of CS 61 or CS 143.


## Textbook
- This course covers both basic networking concepts and advanced cloud networking concepts.
- For basic networking concepts, you can refer to the textbook (K&R): Computer Networking: A Top-Down Approach (7th edition), by Jim Kurose and Keith Ross. Earlier editions are fine. 
- An alternative book is Computer Networks: A Systems Approach (5th edition), by Larry Peterson and Bruce Davie. You can find [an online version](https://proquest-safaribooksonline-com.ezp-prod1.hul.harvard.edu/9780123850591) in Harvard library.
- There are no good textbook for cloud related concepts. You have to refer to my slides and the papers listed in the syllabus for readings. Please contact me if some concepts are hard to understand and I'll provide more supplemental materials.

## Coursework
- Class and biweekly section participation is mandatory.
- Extra credits given based on your contributions to in-class and piazza discussions.
- Programming projects: 70%
  - You will be building an example data center network on your laptop with seven projects, which include topology, routing, load balancing, failure recovery, measurement, and congestion control.
- Midterm exam: 15%
- Scribe: 5%
  - Because there's no good textbook on cloud networking, we plan to create and iterate on a set of course notes that we can reuse in future years. Each student is expected to scribe one lecture. 
- In-class and in-piazza participations 10%
  - including a few cloud news presentations.
- Please refer to the first lecture slides for details.

## Syllabus

| Weeks        | Mon                                                                                                                                                                                                | Tue  | Wed                                                           | Thu                                    | Fri                                         | Sat  | Sun                   |
| :----------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--- | :------------------------------------------------------------ | :------------------------------------- | :------------------------------------------ | :--- | :-------------------- |
| Jan 27-Feb 2 | Course Overview <br> introduction of clouds                                                                                                                                                        |      | Cloud applications I <br> (scalability, low latency)  [**Scribe 1:TBD**]        |     Project 1 released <br> (Setup)                                           |                                             |
| Feb 3-9      | Cloud applications II (bandwidth, reliability, Perf isolation)     [**Scribe 2:TBD**]                                                                                                                                                |      | Basic terms in Networking <br> (IP, MAC, addresses, L2/L3)  [**K&R 4.3**]  |                                        |           Mininet and P4 tutorial                                   |   | Project 1 due 
| Feb 10-16    | Data center topology [**K&R 6.6**] [**Scribe 3**] <br>                                                  |      | Discovery <br> (ARP, DHCP, DNS)     [**K&R 6.4, 6.7, 2.4**]                          |   Project 2 released <br> (Topology )                |                     |
| Feb 17-23    | No class <br> (President's Day)                                                                                                                                                                    |      | Routing basics <br> (link state, distance vector, ECMP, etc.) [**K&R 5.2, 5.3**]   |             |                                             |      |Project 2 Due   |
| Feb 24-Mar 1 | Data Center routing   [**Scribe 4**]                                                                                   |      |  BGP Routing <br> data center BGP routing, Failure recovery    [**K&R 5.4**] [**Scribe 5**]                                                         | Project 3 Released <br> (Routing, ECMP)                    | P4 tutorial continued; ECMP; failure events |      |        |
| Mar 2-8      |          Transport layer and TCP basics [**K&R 3.1, 3.5**]                           |      |      Congestion control and fairness  <br> [**K&R 3.6, 3.7**]]                     | project 4 released (Measurement)                    |                                             |      | Project 3 due         |
| Mar 9-15     |     DataCenterTCP, RDMA  [**Scribe 6**]       |      |   Midterm review                                                           | project 5 released (Failure recovery & ARP)                     |             Measurement and debugging tools                                |      | Project 4 due         |
| Mar 16-22    | no class (Spring recess)                                                                                                                                                                           |      |                                                               |                                        |                                             |      |                       |
| Mar 23-29    |      Midterm exam                                                                        |      | Traffic engineering basics, WCMP [**K&R6.5**] [**Scribe 7**]                                                         | project 6  released <br> (Flowlet)                    |                                 [CONGA](https://people.csail.mit.edu/alizadeh/papers/conga-sigcomm14.pdf) details            |      | Project 5 due         |
| Mar 30-Apr 5 |  VMs, hypervisors, and NIC [**Scribe 8**]    |      |     Traffic shaping & Perf isolation [**Scribe 9**]                                           | project 7  released  <br> (CONGA)                   |                                             |      | project 6  due        |
| Apr 6-12     |      network functions [**Scribe 10**]                     |      |   Load balancing   [**Scribe 11**]                                                         | project 8  released  <br> (SLB) |                                  [Ananta](https://conferences.sigcomm.org/sigcomm/2013/papers/sigcomm/p207.pdf) Details         |   | project 7  due|
| Apr 13-19    |      Switches and P4  [**Scribe 12**]                                                                                                                                                                  |      | Software defined networking   [**K&R 5.5**]                                 |                                        |                                             |  | |
| Apr 20-26    |       WAN (wide-area networking)    [**Scribe 13**]                                                                                                                                                                                         |      | Microsoft Guest Lecture                                       |                                      |                                       Final project suggestions       | | project 8  due|
| Apr 27-May 3 | Security and Ethics  |      |        Course Summary                                                       |                          |                                             |     |     Final project proposal due |
| May 4-10     |                                                                                                                                                                                                    |      |                                                               |                                        |                                             |      |                       |
| May 11-17    |                                                                                                                                                                                                    |      |                                                               |                                        | Final project due                           |      |                       |


<!-- *skim [Jupiter](http://conferences.sigcomm.org/sigcomm/2015/pdf/papers/p183.pdf)*                                    -->


## Diversity and Inclusion
I would like to create a learning environment in our class that supports a diversity of thoughts, perspectives and experiences, and honors your identities (including race, gender, class, sexuality, socioeconomic status, religion, ability, etc.). I (like many people) am still in the process of learning about diverse perspectives and identities. If something was said in class (by anyone) that made you feel uncomfortable, please talk to me about it. If you feel like your performance in the class is being impacted by your experiences outside of class, please don’t hesitate to come and talk with me. As a participant in course discussions, you should also strive to honor the diversity of your classmates. (Statement extracted from one by Dr. Monica Linden at Brown University.)


## Accommodations for Disabilities
If you have a health condition that affects your learning or classroom experience, please let me know as soon as possible. I will, of course, provide all the accommodations listed in your AEO letter (if you have one), but sometimes we can do even better if a student helps me understand what really matters to them. (Statement adapted from one by Prof. Krzysztof Gajos.)