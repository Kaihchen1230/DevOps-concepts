# Definition & Notes

## Software Delivery Cycle

- [SDLC - Overview](https://rb.gy/1wqa6n)
- Software Delivery Life Cycle(SDLC) is a process used by the software industry to design, develop and test high quality softwares. It consists the follow stages:

  1. Planning and Requirement Analysis: done by the senior members of the team by gathering information from different parties, such as cutomers, sales department, market surveys. Those information then used to plan the basic project approachs. Also, to identify risks associated with the project.

  2. Defining Requirements: clearly define the requirements of the project and get approved by different parties, such as customers or the market analysts. Also, complete the SRS (Software Requirement Specification) document.

  3. Designing the Product Architecture: based on the requirements specified in SRS, different approachs for the product architecture is proposed and documented in a DDS - Design Document Specification. Then DDS is reviewed by stakeholders to be further analyzed based on different parameters, such as risk assessment, product robustness, design modularity, budget and time constraints. Then the best design approach is selected and defined all modules and data flows.

  4. Building or Developing the Product: when programmers started to develop the product based on the DDS and following the coding guidelines defined by their organization and programming tools.

  5. Testing the Product: test the product developed by the programmers to find and track different bugs.

  6. Deployment in the Market and Maintenance: release to the public and improve the product based on the feedback from public.

- ![a graphical representation of the various stages of a typical SDLC](https://www.tutorialspoint.com/sdlc/images/sdlc_stages.jpg)

## Test Driven Development

- [Test Driven Development: what it is, and what it is not.](https://www.freecodecamp.org/news/test-driven-development-what-it-is-and-what-it-is-not-41fa6bca02a2/)

- Red Green Refactor cycle:

  - Red: write the test before the actual implementation, which helps the developers to know which functions and classes are necessary

  - Green: write the production code that pass all of test cases in Red phrase. However, the developers don't have to care about best practices.

  - To-do list: all the problems encountered during the Green phrase and the step needed to implement the required features

  - Refactor: make code better while making all the test cases passed.

## Continuous Integration

- [CI/CD | Continuous Integration | Delivery | Deployment](https://www.youtube.com/watch?v=HjXTSbXG1k8)

- when developers merge the code into a shared repositority, then automated tests would be triggered to vertify the merged code.

## Continuous Delivery

- [CONTINUOUS INTEGRATION ESSENTIALS](<https://codeship.com/continuous-integration-essentials#:~:text=Continuous%20Integration%20(CI)%20is%20a,CI%20it%20is%20typically%20implied.>)

- [Continuous Delivery 101 (Part 1)](https://www.youtube.com/watch?v=HnWuIjUw_Q8)

- Automatic testing and automatic deployment on a production ready environment.

- The goal is to ensure the software can be deployed anything by clicking deploy button.

## Configuration Management

- [What is configuration management?](https://www.redhat.com/en/topics/automation/what-is-configuration-management)

- Configuration management is a process for maintaining computer systems, servers, and software in a desired, consistent state. It’s a way to make sure that a system performs as it’s expected to as changes are made over time.

## Containerization

- [Containerization Explained](https://www.youtube.com/watch?v=0qotVMX-J5s)

- Try to fix "it works on my machine"

- Three steps:

  1. manifest: describe the container

  2. image: a read-only template that contains a set of instructions for creating a container that can run on the container platform

  3. container: contains all the libraries or binary needed to run the application

- It is different from VM:

  - different VMs have different OS and each VM has its own binaries and libraries.

  - container is hosting on top of OS. Each container shares the host OS kernel, binaries and libraries. Those components are read-only for each container.

  - container is light-weight compares to VM, because it doesn't have guestOS.

## Cloud Scalability, and Reliability

- [Scalability and Reliability in the Cloud](https://www.slideshare.net/gmthomps/scalability-and-reliability-in-the-cloud)

- [Quora on How does cloud computing improve scalability and reliability and lower the cost of risk mitigation?](https://www.quora.com/How-does-cloud-computing-improve-scalability-and-reliability-and-lower-the-cost-of-risk-mitigation)

- Scalability: the term is used to describe how the application will handle increased loads of traffic volume

  - Vertical: scaling up a single node

  - Horizontal: scaling out acoress multiple nodes

- Reliability: described by the likelihood of failure based on actual measurements

## Software Architecture

- [Software Architecture | Architectural patterns | Architecture vs Design pattern](https://www.youtube.com/watch?v=lTkL1oIMiaU&list=PLSyLGd0D0b4ThfElztKEueqQ5SIHJjUEU&index=1)

- The Architecture is the input of the development phrase in the [SDLC](https://github.com/Kaihchen1230/DevOps-concepts#software-delivery-cycle).

- Software Architecture contains three parts:

  - Architectural Patterns: How the defining overall components of a software system are organized and assembled.

  - Messaging & APIs: How the components communicate with each other.

  - Quality Atrributes(-ilities): The constraints the whole system is ruled by.

- Differnce between architectural pattern and design pattern:

  - **Architectural pattern exists in architecture phrase**, while _Design pattern exists in development phrase_.

  - **Architectural pattern deals with high-level, universal scope**, while _Design pattern deals with lower-level scope_.

  - **Architectural pattern deals with how components are organized** and assembled, while _Design pattern deals with how components are built_.

- Examples of architectural patterns:

  - Client/Server pattern

    - client: the device or program that can make request through the web

      - example: web browser

    - server: a computer program provides functionality and serve other programs/clients

      - type of servers: Apache web servers(serve http requests), database server(run data management server)

      - server is always listening for request, and as soon as it receives one, responds with a message

    - Client/Server pattern work in request(Client), response(Server) cycle via HTTP requests.

    - Client/Server pattern is centralized structure

  - Peer-to-Peer

    - Peer-to-Peer is decentralized strcture
    - no client and no server
    - both devices can be reqestor and response providers
    - each one is able to send and receive data directly with one another
    - examples of Peer-to-Peer:
      - BitTorrent protocol: a communication protocol for file sharing
      - videochat protocol

  - Monolithic:

  - Microservices:

  - REST:
