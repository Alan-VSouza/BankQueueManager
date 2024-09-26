# 🏦 Bank Queue - Practical Assignment 04

This project implements a queue system for bank customer service, where clients can be divided into two queues: **General** and **Priority**. The system simulates customer service according to priority rules and allows users to add clients, serve them, and finish the workday interactively.

## ✨ Features
- **Queue Management**: Handles two queues—one for general clients and one for priority clients.
- **Priority-Based Service**: Clients in the priority queue are served before those in the general queue.
- **Interactive Commands**: Users can input commands to add clients to queues, free up cashiers for service, or end the workday.
- **Service Order Output**: Displays the order in which clients were served when the workday ends.

## 👥 Team Members
- Alan Andrade Vasconi de Souza - SC3038319
- Felipe Santos Lourenço - SC303867X
- Fernando Henrique de Castro Chagas - SC3037495

## 🛠️ How to Compile

To compile the project, ensure you have GCC installed. Then, simply run the following command in the terminal:

```
make
```
## 🚀 How to Run

After compilation, execute the program with:

```
./bank_queue
```

## 📥 Input Commands

- **g name:** Adds a general client with the specified name to the queue.
- **p name:** Adds a priority client with the specified name to the queue.
- **s:** Simulates freeing up a cashier and calls the next client according to priority.
- **f:** Ends the workday and prints the order in which clients were served.

## 💡 Example of Usage
**Input:**

```
g Alan
p Bruno
g Cézar
s
g Douglas
s
p Ernesto
s
f
```

**Output:**

```
Bruno
Alan
Ernesto
```

## 📂 Project Structure

- **main.c:** Main program file that handles user interactions.
- **queue.c:** Implementation of queue-related functions.
- **queue.h:** Declarations of structures and queue management functions.
- **makefile:** Script to compile the project and generate the executable.

## 🧹 Cleaning the Project
To remove object files and the executable, use the following command:

```
make clean
```