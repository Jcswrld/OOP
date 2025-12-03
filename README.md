<h1 align="center">Task and To-Do List Manager</h1>
<h3 align="center">Your console-based Task and To-Do List Manager.</h3>
<h5 align="center">IT 2110</h5>
<h5 align="center">Ramirez, Jhon Victor E.</h5>
<h5 align="center">Egle, Keihl Axell B.</h5>
<h5 align="center">Mayuga, Mark Jc B.</h5>
<h5 align="center">MAranan, Lloyd Rasmus</h5>

<h2>‧₊˚ ┊ Overview</h2>


<h5>Task and To-Do List Manager is a console-based Java application that lets users create, organize, and manage tasks through the terminal. It applies core OOP concepts like abstraction, inheritance, and encapsulation, and provides essential features such as adding, editing, sorting, and deleting tasks for efficient task management.</h5>

<h3>User can:</h3>
<h5>✏️ Add new tasks</h5>
<h5>📔 View all tasks</h5>
<h5>⏳ View pending tasks</h5>
<h5>✅ View completed tasks</h5>
<h5>🔄 Mark tasks as completed or pending</h5>
<h5>✍🏻 Edit tasks</h5>
<h5>📑 Sort tasks by deadline, priority, or category</h5>
<h5>🗑️ Delete tasks</h5>
<h5>🚪 Exit the application</h5>

<h3>Note Entry Storage</h3>
<h5>💾 All entries are stored in a plain text file.</h5>

<h2>‧₊˚ ┊ Project Structure</h2>

<pre>
📂 src/
└── 📂 oop/
    ├── ☕ Main.java
</pre>
<h5>Main.java -  Entry point of the program, containing the menu and handles user interactions.</h5>
<h3>How to run the program:</h3>
<h5>1.	Open the folder OOP</h5>
<h5>2.	Run main.java</h5>

<h2>‧₊˚ ┊  Features</h2>

<h5>Add new tasks – Lets you create a new task by entering its title, category (work, personal, or other), deadline, and priority (low, medium, high). The task is then added to your list.</h5>
<h5>View all tasks – Displays every task you’ve added, showing its type, deadline, priority, and whether it’s completed or not.</h5>
<h5>View pending tasks – Shows only the tasks that are not yet completed, helping you focus on what still needs to be done.</h5>
<h5>View completed tasks – Shows only the tasks you have marked as completed, so you can track what’s already finished.</h5>
<h5>Mark tasks as completed or pending – Lets you change a task’s status: mark it as completed when done, or mark it back as pending if it’s not finished.</h5>
<h5>Edit tasks – Allows you to update a task’s details like its title, category, deadline, or priority without creating a new task. Sort tasks by deadline, priority, or category – Organizes your tasks for easier viewing.</h5>
<h5>Deadline – Sorts tasks from earliest to latest.</h5>
<h5></h5>
<h5>Priority – Sorts tasks from high → medium → low.</h5>
<h5>Category – Sorts tasks alphabetically (Work, Personal, Other).</h5>
<h5>Delete tasks – Removes a task completely from your list.</h5>
<h5>Exit the application – Closes the program safely.</h5>

<h2>‧₊˚ ┊  Object-oriented Principles</h2>

<h5><strong>💊Encapsulation:</strong><br>
Encapsulation is implemented through the use of private fields in the Task class, such as title, category, deadline, priority, and completed, and controlled access through public getters and setters. This ensures that the internal state of a task cannot be modified directly from outside the class, keeping data safe and consistent. For example, you can update a task’s title or priority only via its setter methods, which enforces controlled access to the data.
</h5>

<hr>

<h5><strong>💡Abstraction:</strong><br>
Abstraction is achieved through the abstract class Task and its abstract method displayTask(). The Task class defines the general structure and behavior of a task, but it does not get instantiated directly. Instead, concrete subclasses like WorkTask, PersonalTask, and OtherTask implement the displayTask() method in their own way. This hides unnecessary implementation details and exposes only the essential features to the rest of the system.
</h5>

<hr>

<h5><strong>🧬Inheritance:</strong><br>
Inheritance is used by creating subclasses (WorkTask, PersonalTask, OtherTask) that inherit common properties and methods from the Task class. This avoids code duplication, as all shared behavior—like handling title, deadline, priority, and completion status—is already defined in the parent class. Subclasses can also extend or specialize behavior if needed, making the system easier to maintain and extend.
</h5>

<hr>

<h5><strong>🎭Polymorphism:</strong><br>
Polymorphism is applied through method overriding in the subclasses. All task types implement their own version of displayTask(), but the program can call this method on a Task reference without knowing its specific type. For instance, in viewTasks(), calling tasks[i].displayTask(i + 1) automatically executes the correct method for WorkTask, PersonalTask, or OtherTask. This allows flexible code that can handle different task types in a uniform way.
</h5>

<h2>‧₊˚ ┊  Example Output</h2>

<pre>
=== TASK & TO-DO LIST MANAGER ===
1. Add Task
2. View All Tasks
3. View Pending Tasks
4. View Completed Tasks
5. Mark Task as Completed / Pending
6. Edit Task
7. Sort Tasks
8. Delete Task
0. Exit
Choose an option: 
</pre>



    
    

