# Task Management Bash Script

## Introduction

This project is a simple task management system implemented as a Bash script. It is designed to provide a command-line interface for managing tasks, making it ideal for users who prefer to work in a terminal environment. Despite its simplicity, it offers a range of features typically found in more complex task management systems.

## Design Choices

### Data Storage

The tasks are stored in a CSV file named `tasks.csv`. Each task is represented as a row in the CSV file, with columns for the task ID, title, due date, description, location, priority, and completion status. This format was chosen for its simplicity and ease of use with standard Unix utilities such as `awk` and `sed`.

### Code Organization

The code is organized into functions, each of which performs a specific task such as creating a task, updating a task, deleting a task, listing all tasks, searching for a task, or marking a task as completed. This modular design makes the code easier to understand and maintain.

## Features

### Create a Task

Users can create a new task by entering details such as the title, due date, description, location, and priority. The script will prompt the user for each of these details, ensuring that all necessary information is captured.

### Update a Task

Users can update an existing task by entering the task ID and the new details. The script will prompt the user for each detail, allowing them to change any aspect of the task. This makes it easy to adjust task details as circumstances change.

### Delete a Task

Users can delete an existing task by entering the task ID. This is a straightforward operation, but it should be used with caution, as deleted tasks cannot be recovered.

### List All Tasks

Users can list all tasks, which will be displayed in a user-friendly, column-aligned format. This provides a quick and easy way to view all tasks at a glance.

### Search for a Task

Users can search for tasks by entering a search term. The script will search all fields of all tasks for the search term, providing a powerful tool for finding specific tasks.

### Mark a Task as Completed

Users can mark a task as completed by entering the task ID. The completion status of the task will be updated to "Completed". This provides a satisfying way to mark the end of a task.

## Usage

To use this script, simply run it in a Bash shell:

```shellscript
/bin/bash /path/to/taskm.sh
