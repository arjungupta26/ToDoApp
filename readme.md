# Java Swing To-Do List Application
## 1. Project Overview
   This is a simple, yet functional, desktop To-Do List application built using Java's Swing GUI toolkit. It provides a clean user interface for users to add, view, and delete their daily tasks. The primary goal of this project is to demonstrate fundamental concepts of GUI development in Java.

## 2. Features
   - Add Tasks: Easily add new tasks to your list via a text input field.

- View Tasks: All tasks are displayed in a clear, scrollable list.

- Delete Tasks: Select any task from the list and remove it with a single click.

- User-Friendly Interface: A clean, intuitive, and straightforward layout.

- Input Validation: Prevents the user from adding empty tasks.

- User Feedback: Provides simple dialog boxes for errors (e.g., trying to delete without selecting a task).

## 3. Technologies Used
   - Language: Java

- GUI Toolkit: Java Swing

- IDE: Compatible with any standard Java IDE like IntelliJ IDEA, Eclipse, or VS Code.

## 4. How to Run the Application
   #### Prerequisites
   - Java Development Kit (JDK) 8 or higher installed on your system.

- A Java IDE (recommended) or command-line tools for compilation and execution.

#### Steps:
- Download the Code:
- Save the ToDoApp.java file to your local machine.

- Compile the Code:
Open a terminal or command prompt, navigate to the directory where you saved the file, and run the following command:

  - javac ToDoApp.java

- Run the Application:
After a successful compilation (which creates a ToDoApp.class file), run the application with this command:

  - java ToDoApp

- The application window should now appear on your screen.

## 5. Code Structure (ToDoApp.java)
   The entire application is self-contained within the ToDoApp.java file. Here is a brief breakdown of its structure:

### ToDoApp class:

- Extends JFrame to serve as the main application window.

- The constructor ToDoApp() initializes the entire GUI, sets up layouts, and attaches event listeners.

### GUI Components:

JFrame: The main window.

DefaultListModel<String>: The data model that holds the list of tasks. This allows for dynamic addition and removal of elements.

JList<String>: The visual component that displays the tasks from the DefaultListModel.

JTextField: The input field for typing new tasks.

JButton: Used for the "Add Task" and "Delete Selected Task" actions.

JPanel: Used to group and organize other components within the frame, using layouts like BorderLayout, GridLayout, and FlowLayout.

JScrollPane: Wraps the JList to provide scrolling capabilities when the task list becomes long.

### Event Handling:

ActionListener interfaces are used to handle user actions (button clicks, pressing Enter).

The "Add" functionality is triggered by both the "Add Task" button and pressing the 'Enter' key in the text field.

The "Delete" functionality is triggered by the "Delete Selected Task" button, which removes the currently highlighted item in the JList.

main Method:

This is the entry point of the application.

- It uses SwingUtilities.invokeLater() to ensure that the GUI is created and updated on the Event Dispatch Thread (EDT), which is the standard and safe way to work with Swing.