tasks = []

def add_task(task):
    tasks.append(task)
    print("Task added successfully.")

def remove_task(task_index):
    if task_index < len(tasks):
        del tasks[task_index]
        print("Task removed successfully.")
    else:
        print("Invalid task index.")

def list_tasks():
    if tasks:
        print("Your To-Do List:")
        for i, task in enumerate(tasks):
            print(f"{i + 1}. {task}")
    else:
        print("Your To-Do List is empty.")

# Example usage
add_task("Buy groceries")
add_task("Finish homework")
list_tasks()
remove_task(1)
list_tasks()
