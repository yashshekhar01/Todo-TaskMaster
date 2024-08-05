# TaskMaster

## Overview

**TaskMaster** is a modern to-do list application developed using React and Vite, with styling provided by Tailwind CSS. The application is designed to help users manage their tasks efficiently by offering features such as task addition, editing, deletion, and toggling completion status. It uses local storage to persist tasks across browser sessions.

### System Design

The application follows a component-based architecture:

- **Components**: The primary components include `Navbar` and the main `App` component.
- **State Management**: Utilizes React's `useState` and `useEffect` hooks for managing and persisting state.
- **Local Storage**: Tasks are stored in the browser's local storage to ensure data persistence.
- **Styling**: Tailwind CSS is used for responsive and modern styling.

## Implementation

### Core Features

1. **Add a Task**: Users can input a task description and save it to the list.
2. **Edit a Task**: Users can modify the text of existing tasks.
3. **Delete a Task**: Users can remove tasks from the list.
4. **Toggle Task Completion**: Users can mark tasks as completed or not completed.
5. **Show/Hide Completed Tasks**: Users can choose to show or hide completed tasks.

### Key Components

- **`App.jsx`**: The main component managing the application state and functionality. It includes:
  - State variables for managing tasks (`todos`), current task input (`todo`), and visibility of completed tasks (`showFinished`).
  - Functions for handling task addition, editing, deletion, and completion toggling.
  - `useEffect` hook for loading tasks from local storage on component mount.
  
- **`Navbar`**: A component for navigation (if applicable).

### Data Flow

1. **Adding a Task**: Updates the `todos` state and saves to local storage.
2. **Editing a Task**: Updates the `todos` state and saves the changes to local storage.
3. **Deleting a Task**: Removes the task from the `todos` state and updates local storage.
4. **Toggling Completion**: Updates the `isCompleted` status of a task and reflects this change in local storage.
5. **Visibility Toggle**: Controls whether completed tasks are shown based on user preference.
   

## Setup and Running

Follow these steps to set up and run the TaskMaster application:

### 1. Clone the Repository

Open your terminal and run the following command to clone the repository:

```bash
git clone https://github.com/yashshekhar01/Todo-TaskMaster.git


## Installation and Running

Follow these steps to clone and run the TaskMaster application on your local machine:

### 1. Clone the Repository

Open your terminal and run the following command to clone the repository:

git clone https://github.com/yashshekhar01/Todo-TaskMaster.git

2. Navigate to the Project Directory
   
Change to the project directory:

cd Todo-TaskMaster

3. Install Dependencies
   
Ensure you have Node.js and npm (Node Package Manager) installed. Then install the project dependencies by running:

npm install

4. Run the Application
   
Start the development server with Vite:

npm run dev

This will start the application and you should see output indicating that the server is running, along with a local development URL (typically http://localhost:3000).

5. Open the Application
Open your web browser and navigate to http://localhost:3000 or the localhost which shows in the termianl, just click, view and interact with the TaskMaster application.

## Project Structure

src/ - Contains the source code of the application.
components/ - Contains reusable React components such as Navbar.
App.jsx - The main React component that holds the core functionality of the application.

## Dependencies

React: A JavaScript library for building user interfaces.
Vite: A fast build tool and development server.
Tailwind CSS: A utility-first CSS framework for styling.
React Icons: A library for including popular icons.
