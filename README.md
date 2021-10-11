# Space Management with Django

A small web application to manage your tasks

![gifspace](https://user-images.githubusercontent.com/65988061/136683114-bddefaf3-73ab-4892-be69-ed0f3835050a.gif)

## Content

[1. Domain](#1-Domain)

&nbsp;&nbsp;[1.1 Description](#11-description)

&nbsp;&nbsp;[1.2 CRC Model](#12-CRC-Model)

&nbsp;&nbsp;[1.3 Event Storming](#13-Event-Storming)

[2. Architecture](#2-Architecture)

&nbsp;&nbsp;[2.0 C4 Model](#20-C4-model)

&nbsp;&nbsp;[2.1 System Container Context C1-C2](#21-System-container-context-c1-c2)

[3. How to run](#3-How-to-run)

&nbsp;&nbsp;[3.1 Installation](#31-installation)

[4. Inspiration](#4-inspiration)

## 1. Domain

### 1.1 Description

**Definition:**

> Domain - A sphere of knowledge, influence, or activity. The subject area to which the user applies a program is the domain of the software. [Domain-Driven Design Reference](http://domainlanguage.com/ddd/reference/), Eric Evans

**Main reasons for selecting this domain:**

- It is common to have different tasks throughout the day.
- It is not easy to remember everything we have to do.
- It's a simple project with which I can learn a little more about Django.
- This project can help people to manage their day to day life.

**Tasks and users**

The main project entitie are `tasks` and `users`. A person becomes a `user` by registering.

A `task` can be created by a `user`.

A `task` can be deleted by a `user`.

A `task` can be updated by a `user`.

A `user` can have multiple `tasks`.

### 1.2 CRC Model

**Definition:**

> CRC Model - A CRC model is a collection of CRC cards that represent whole or part of an application or problem domain. The most common use for CRC models, the one that this white paper addresses, is to gather and define the user requirements for an object-oriented application. [CRC Modeling: Bridging the Communication Gap Between Developers and Users](http://www.uml.org.cn/umlapplication/pdf/crcmodeling.pdf)

### 1.3 Event Storming

There are many ways to show behavior and events. One of them is a light technique called [Event Storming](https://www.eventstorming.com/) which is becoming more popular. Below are presented 2 main business processes using this technique: user registration and tasks.

Note: Event Storming is a light, live workshop. One of the possible outputs of this workshop is presented here. Even if you are not doing Event Storming workshops, this type of process presentation can be very valuable to you and your stakeholders.

**User Registration and Task Management process**

------

![flow](https://user-images.githubusercontent.com/65988061/136731759-72ad429f-3322-4404-a046-eec27e5ededf.png)


## 2. Architecture

### 2.0 C4 Model

[C4 model](https://c4model.com/) is a lean graphical notation technique for modelling the architecture of software systems. <br>

As can be found on the website of the author of this model ([Simon Brown](https://simonbrown.je/)): *The C4 model was created as a way to help software development teams describe and communicate software architecture, both during up-front design sessions and when retrospectively documenting an existing codebase* <br>

*Model C4* defines 4 levels (views) of the system architecture: *System Context*, *Container*, *Component* and *Code*. Below are examples of each of these levels that describe the architecture of this system. **In this example I will use a hybrid of system context (C1) and container (C2) for the simplicity of the application.** <br>

### 2.1 System Container Context C1-C2

![diagram](https://user-images.githubusercontent.com/65988061/136727370-8d2ad1f9-ad6b-4afe-94ac-c4258dd66540.png)

## 3. How to run

### 3.1 Installation

1. Clone the repo
   ```py
   git clone https://github.com/joseluistello/ToDo-List.git
   ```

2. Create Virtual Enviroment
   ```py
   cd ToDoList
   ```
   ```py
   virtualenv venv
   ```
   
3. Run Virtual Enviroment
   ```py
   venv\Scripts\activate
   ```
   
4. Install Django
   ```py
   pip install Django
   ```

5. Run Django 
   ```py
   python manage.py runserver
   ```


## 4. Inspiration

[kamil Grzybek](https://github.com/kgrzybek/modular-monolith-with-ddd)


<!-- CONTACT -->
## Contact

José Luis Tello - [@jotaele_tello](https://twitter.com/jotaele_tello) - joluistello@gmail.com
