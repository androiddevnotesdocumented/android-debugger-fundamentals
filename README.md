## Documented

## Important points

### Getting started

Attach a Debugger to the process

Restart app by clicking Debug green icon

If you see, Waiting for Debugger in your Android device, it worked.

### What is breakpoint?

A breakpoint is a place in your code where you want to pause the normal execution of your app to perform other actions such as examining variables or evaluating expressions, or executing your code line by line to determine the causes of runtime errors. You can set a breakpoint on any executable line of code.

![](https://developer.android.com/codelabs/android-training-using-debugger/img/472679cda2419269.png)

The figure above shows the **Debug** pane with the **Debugger** and **Console** tabs. The **Debugger** tab is selected, showing the **Debugger** pane with the following features:

1.  **Frames** tab: Click to show the **Frames** pane with the current execution stack frames for a given thread. The execution stack shows each class and method that have been called in your app and in the Android runtime, with the most recent method at the top.

Right click on Frames -> Layout -> Threads for threads tab to show

Click the **Threads** tab to replace the **Frames** pane with the **Threads** pane. Your app is currently running in the main thread, and that the app is executing the `compute()` method in `MainActivity`.


*   **Watches** button: Click to show the **Watches** pane within the **Variables** pane, which shows the values for any variable watches you have set. Watches allow you to keep track of a specific variable in your program, and see how that variable changes as your program runs.

1.  **Variables** pane**:** Shows the variables in the current scope and their values. At this stage of your app's execution, the available variables are: `this` (for the `Activity`), `operator` (the operator name from `Calculator.Operator` that the method was called from), as well as the global variables for the `EditText` elements and the `TextView`. Each variable in this pane has an expand icon to expand the list of object properties for the variable. Try expanding a variable to explore its properties.

### Resume App Execution

Resume your app's execution by choosing **Run > Resume Program**, or click the **Resume** ![or click the Resume [ICON HERE] icon on the left side of the debugger window. [IMAGEINFO]: ic_resume.png, Resume icon](https://developer.android.com/codelabs/android-training-using-debugger/img/1c83d051db67e1dc.png) icon on the left side of the debugger window.


The SimpleCalc app continues running, and you can interact with the app until the next time the code execution arrives at the breakpoint.