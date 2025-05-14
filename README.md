## 📘 Overview
This OS Simulator is a terminal-based project which simulates the core behavior of an operating system, including process creation, multitasking, resource allocation, user/kernel modes, and scheduling — all built without actual hardware-level control, purely in a simulated environment.

The system runs through a CLI (command-line interface), emulates booting behavior, and launches independent tasks. It mimics how an operating system manages memory, CPU cores, and storage to support multiple simultaneous user processes.

---

## ⚙️ Main Features

### 🔧 OS Boot & Setup
- Displays a custom OS name 'jigglyOS' and boot animation with timed delays.
- At startup, users input system configuration:
  - **RAM size**
  - **Hard Drive capacity**
  - **Number of CPU cores**

These values are used to simulate resource availability and allocation for tasks.

### 👤 User Mode vs Kernel Mode
- **User Mode:** Allows users to launch, minimize, and switch between tasks.
- **Kernel Mode:** Gives low-level control such as terminating all processes from the ready queue.

### 🧵 Process Management
- Each task is executed in its own terminal.
- RAM and hard drive space are checked before launching tasks.
- When tasks terminate, resources are released automatically.
- Utilizes First-Come First-Served (FCFS) scheduling algorithm.
- Threading and synchronization handled via:
  - **Semaphores**

---

## 📂 Task List (15 Total)

Each of the following tasks is independently launched and managed like a real OS process:
1. **Notepad** – Simple text input with saving.
2. **Calculator** – Basic arithmetic operations.
3. **Create File** – Make a new file.
4. **Copy File** – Duplicate an existing file.
5. **Rename File** – Rename files.
6. **Delete File** – Remove files permanently.
7. **Tic Tac Toe Game** – Two-player console-based game.
8. **Temperature Calculator** – Convert between Celsius and Fahrenheit.
9. **Reverse String** – Input a string and view its reverse.
10. **Letter Count** – Count letters in a string.
11. **Age Calculator** – Calculate age from birth year.
12. **Play Song** – Simulate music with system beeps.
13. **Number Guessing** – Guess a randomly chosen number.
14. **Gender Guessing** – Game that guesses gender from questions.
15. **Download** – Simulate a file download with a progress bar.

---

## 📦 Technologies Used
- **C**
- **VMware based Ubuntu**

---

### Instructions (Ubuntu terminal):
gcc project.c -lncurses -o project -pthread
./project.c
