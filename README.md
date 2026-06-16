# Matlab_Study

Matlab study


## How to start

### Matlab onramp in Matlab online courses


### When you enter a command without a semicolon at the end, MATLAB displays the result.

EX: 

TASK 2

Assign the result of 3*5 to a variable named m

m = 3*5 

TASK 3

Enter the command m = m + 1 to see what happens.

<img width="334" height="214" alt="Screenshot 2026-05-10 at 12 16 56 pm" src="https://github.com/user-attachments/assets/7be7a44b-fc14-4a94-b4e1-12d2a058576f" />


TASK 4

Create a variable named y that has the value of m/2.

<img width="358" height="252" alt="Screenshot 2026-05-10 at 12 17 59 pm" src="https://github.com/user-attachments/assets/b2e98e34-9720-4874-8541-86a7dfcf4119" />


### To add a semicolon to the end of a command so that the result is not displayed. MATLAB still executes the command, and you can see the variable in the Workspace panel.

EX: 

TASK 5

Enter k = 8 - 2; 

including the semicolon at the end.

**The result won't appear in the Command Window, but you can see the value of k in the Workspace panel.**


<img width="314" height="112" alt="Screenshot 2026-05-10 at 12 30 17 pm" src="https://github.com/user-attachments/assets/f6aa617b-6da5-4d14-bf33-deebc7e54cd6" />


<img width="462" height="368" alt="Screenshot 2026-05-10 at 12 30 57 pm" src="https://github.com/user-attachments/assets/62cfed44-0acb-4c5e-a500-8d0b0c4f0a88" />


### You can recall previous commands by pressing the Up arrow key ↑ on your keyboard. 

### Note. Command Window must be the active window for this keystroke to work.

EX: 

TASK 6

Press the Up arrow key to return to the command m = 3*5, and before pressing Enter, edit the command to be m = 3*k.


<img width="1012" height="368" alt="Screenshot 2026-05-10 at 12 32 15 pm" src="https://github.com/user-attachments/assets/54f23b7a-2989-4ba0-a01f-d8c1ad99a7c8" />


### When you enter just a variable name at the command prompt, MATLAB displays the current value of that variable.

TASK 7

In Task 4, you calculated the value of y using the value of m. Was y recalculated when you modified m in Task 6?

Type just the variable name y at the command prompt, and press Enter.

<img width="340" height="250" alt="Screenshot 2026-05-10 at 1 56 53 pm" src="https://github.com/user-attachments/assets/95ad980c-4e4a-4785-a005-3097caf3655f" />


# Name Variables

### You can name your MATLAB variables anything you'd like as long as they start with a letter and contain only letters (A-Z, a-z), numbers, and underscores (_). *(MATLAB variables are also case sensitive)*

EX: 

TASK 1

Create a variable named A with the value -2.

<img width="336" height="408" alt="Screenshot 2026-05-10 at 2 01 24 pm" src="https://github.com/user-attachments/assets/974828f7-bbf8-447d-a33b-17ad453f308a" />

<img width="470" height="276" alt="Screenshot 2026-05-10 at 2 01 30 pm" src="https://github.com/user-attachments/assets/922968d5-8d07-437e-9442-d1fd3094b1d7" />

Task 2

Use A and a to calculate 

a+A / 2

Store the result in a variable named meanAa.

<img width="520" height="484" alt="Screenshot 2026-05-10 at 2 03 41 pm" src="https://github.com/user-attachments/assets/35e4cd06-31fa-4d8a-9cf8-840787580cb0" />

Task 3

If you use an invalid variable name, MATLAB displays an error message and a suggested correction. You can use this correction, modify it, or press Esc to delete the suggestion.

<img width="650" height="336" alt="Screenshot 2026-05-10 at 2 06 00 pm" src="https://github.com/user-attachments/assets/8bb18da4-c788-46ec-b16b-8bdc7f037cb0" />


# Save and Load Variables

### You can save variables in your workspace to a MAT-file, a file format specific to MATLAB, by using the save command.

### For example, to save all the variables in the workspace to a MAT-file named filename.mat, use the command:

### >> save filename

Task 1

<img width="788" height="190" alt="Screenshot 2026-05-10 at 2 07 44 pm" src="https://github.com/user-attachments/assets/831ca738-5bbc-4bda-b2ae-4365a47b9fa7" />


### To remove all the variables from your workspace with the *clear command*.

EX: 
>> clear

### To load variables from a MAT-file, use the load command.

>> load filename

EX: 

Task 3 

Load the variables from the file datafile.mat.

<img width="528" height="82" alt="Screenshot 2026-05-10 at 2 10 50 pm" src="https://github.com/user-attachments/assets/63deb646-72a0-4732-9fda-df40dbbd4148" />

<img width="502" height="222" alt="Screenshot 2026-05-10 at 2 10 55 pm" src="https://github.com/user-attachments/assets/583c9230-98d6-4c70-adb4-277135a93f42" />

### To see the contents of any variable by entering the name of the variable in the Command Window: 

### >> *Variable name*

EX:

<img width="774" height="426" alt="Screenshot 2026-05-10 at 2 12 37 pm" src="https://github.com/user-attachments/assets/f5547fb3-e2e3-40d3-be2e-0e0211ea75f1" />


### The clear command cleans up the workspace. You can use the clc command to clean up the Command Window.

<img width="2394" height="950" alt="Screenshot 2026-05-10 at 2 18 53 pm" src="https://github.com/user-attachments/assets/5c4b4345-4b7e-4089-b3fa-7cb504a38130" />


### Before closing MATLAB, you can use MAT-files to save your variables. You can then load the variables into the workspace when you reopen MATLAB.

### To load or save only some of your variables, you can use additional inputs with the commands.

The provided file myData.mat contains multiple variables. Try loading just the variable k.
>> load myData k

Then try saving the variable k to a new MAT-file named justk.mat.

## Curiosity. Does that mean the variable 'k' is inside myData.mat and it will pick up with the data called 'k'?

### 1. The Meaning of load myData k

A file named myData.mat might contain various variables like a, b, c, and k. Running simply load myData will import all those variables into your Workspace at once.

However, entering load myData k commands MATLAB to:

  1. Search through the *myData.mat file*.

  2. Extract only the specific *variable k*.

  3. Load it into your current Workspace.

### 2. The Meaning of save justk k

Assuming the *variable k* is now active in your Workspace, executing this command tells MATLAB to:

Create a new file named justk.mat. <- Name doesn't need to be followed in this format; however, you need to follow the rules that 

# >> save (file name) (variable)

Take the value of the variable k from the Workspace and save it in this new file.

Note. This targeted approach is highly useful when you need to isolate specific data from a large file containing hundreds of variables, or when you only want to save particular results separately without cluttering your storage.


## Curiosity 2. What will happen if I use the 'save' command before 'load'? 

If you use the `save` command before `load`, the result depends entirely on the current state of your Workspace (memory). This can be broken down into three main scenarios:

### 1. When the Workspace is Empty

If you just opened MATLAB or used the `clear` command, your Workspace will be empty.

* **Command:** `save testfile k`
* **Result:** An error occurs.
* **Reason:** MATLAB recognises that the variable `k` does not exist anywhere in its active memory. It is impossible to save a variable that hasn't been defined yet.

### 2. When You Create a Variable Manually

You can use `save` without `load` if you declare the variable directly in the Command Window first.

* **Command:**
```matlab
>> myValue = 100;
>> save myNewFile myValue

```


* **Result:** It is saved successfully.
* **Reason:** Whether a variable is imported via `load` or created manually by you, the only requirement is that the target variable must exist in the Workspace memory before saving.

### 3. Using `save` with a Filename but No Variable Names

This situation requires the most caution.

* **Command:** `save backup`
* **Result:** MATLAB saves *all* variables currently active in the Workspace into `backup.mat`.
* **Risk:** If the Workspace is empty, it creates an empty file. However, if you have numerous variables loaded in the background, all of them are saved simultaneously, which can result in an unnecessarily large file size.

---

### 💡 Summary

* The `save` function transfers variables currently active in your Workspace into a file.
* It does not matter whether the data was imported (`load`) or manually created.
* Attempting to save a variable name that does not exist in the Workspace will always result in an error.


# Use Built-in Functions and Constants

MATLAB contains built-in constants, such as pi to represent π.
>> a = pi

>> a =  3.1416

Although the Command Window output shows only four decimal places for pi, MATLAB internally represents the built-in constant with more decimal places.

TASK1 

Create a variable named x with a value of π/2.

<img width="580" height="306" alt="Screenshot 2026-05-12 at 9 27 57 pm" src="https://github.com/user-attachments/assets/d2109011-d6a4-43ae-99b9-fa317fac4652" />



MATLAB contains a wide variety of built-in functions, such as abs (absolute value) and eig (eigenvalues).

>> a = sin(-5)

a =  0.9589

Pass inputs to functions by using parentheses, similar to function notation in math.


TASK 2

Calculate the sine of x by using the sin function. Assign the result to a variable named y.

<img width="470" height="264" alt="Screenshot 2026-05-12 at 9 32 47 pm" src="https://github.com/user-attachments/assets/e03eb4d9-64b0-46b5-a15d-01b95e3cbe1c" />

TASK 3

Calculate the square root of -9 by using the sqrt function. Assign the result to a variable named z.

<img width="496" height="266" alt="Screenshot 2026-05-12 at 9 33 58 pm" src="https://github.com/user-attachments/assets/b1e87e82-48d6-42d5-996e-72f0d61d83f3" />


Note. the solution contains the imaginary number i : a built-in constant in MATLAB

The Command Window output shows only the first four decimal places. 

You can control the displayed precision with the format function.


Task 4

Try displaying more decimal places of the variable x using:

<img width="558" height="252" alt="Screenshot 2026-05-12 at 9 36 10 pm" src="https://github.com/user-attachments/assets/21337b53-bdfa-45b9-a0f5-50528d8b8ce6" />

<img width="420" height="252" alt="Screenshot 2026-05-12 at 9 36 21 pm" src="https://github.com/user-attachments/assets/5a4a8b47-79e6-46b9-befb-0051ba8c0223" />


## Curiosity 1. Can't I specify a random number of decimal places while using this function; "format long/short"? 

You cannot use it to specify a random number of decimal places (like "exactly 7" or "exactly 10").

### 1. The Fixed Standards of format
  
  * The format command changes the display mode for the entire Command Window session.
    
  *It follows these hard-coded rules:


<img width="1464" height="394" alt="Screenshot 2026-05-12 at 9 44 49 pm" src="https://github.com/user-attachments/assets/ea3f0e1c-76a9-4194-bd1b-24065b33ba64" />

### 2. How to specify a custom number of places

If you want to decide exactly how many digits to display, you need to use formatted output functions rather than global display settings. The most common tool for this is fprintf.

If you wanted to see exactly 7 decimal places, you would use:

>> x = pi;
>> fprintf('%.7f\n', x)
3.1415927



%: Starts the formatting command.

.7: Tells MATLAB to show exactly 7 digits after the decimal point.

f: Stands for "fixed-point" notation.


### 3. Why doesn't the format allow custom numbers?

The format command is designed for UI convenience, not for reporting data.

**format short** is meant to keep the screen clean so you can see many numbers at once without them wrapping to the next line.

**format long** is meant to show you the full precision of a "double" (the default data type in MATLAB) to check for rounding errors.


### Crucial Note: Changing the format never changes the actual value of the variable in memory. MATLAB always calculates with maximum precision (~16 digits) regardless of whether you are looking at 4 digits or 15.


# The MATLAB Editor

<img width="2118" height="730" alt="Screenshot 2026-05-13 at 3 19 02 pm" src="https://github.com/user-attachments/assets/232e5415-619c-48cf-8fc6-6baa7ad3c3f3" />


## TASK 1. 

Run the script to populate the output pane.

Then modify the command for Task 1 so that r has a value of 0.5.

<img width="2036" height="668" alt="Screenshot 2026-05-13 at 3 21 28 pm" src="https://github.com/user-attachments/assets/f322b583-80ff-4e2b-8675-7aa1c3510348" />

<img width="2062" height="1006" alt="Screenshot 2026-05-13 at 3 21 45 pm" src="https://github.com/user-attachments/assets/f015959b-8fc8-4d8f-9ba6-ecb881205ba2" />

## TASK 2.

To execute the code for just one section, click the  Run Section button in the MATLAB Toolstrip.

Try changing the value of r and running only that section. What happens to the value of r in the output pane? What about the value of x?

You can also use the buttons in the toolstrip to switch between text and code.

# Put your cursor at the end of the last line of code, then try adding a new section using the Section Break button. 

## When I press the section break button: 

<img width="1372" height="822" alt="Screenshot 2026-05-13 at 3 31 53 pm" src="https://github.com/user-attachments/assets/5d662a3c-1932-46a0-b0fe-bea01e85d3ba" />


# Use the Live editor text icon Text button and insert the text "Calculate Circumference". 

## When I press the text button: 

<img width="1222" height="842" alt="Screenshot 2026-05-13 at 3 33 35 pm" src="https://github.com/user-attachments/assets/8bcbe6fa-dcce-4a33-82e6-8338b1776491" />


# Finally, use the Live editor code icon Code button and add the code y = 2*pi*r.

## When I press the code button:

<img width="1206" height="856" alt="Screenshot 2026-05-13 at 3 34 44 pm" src="https://github.com/user-attachments/assets/aa501816-2dcd-4b37-b7da-0c8d4acf709d" />

## Add the code y = 2*pi*r : 

<img width="2062" height="1046" alt="Screenshot 2026-05-13 at 3 35 17 pm" src="https://github.com/user-attachments/assets/b2064ca5-7452-42a9-9922-9b55732a335f" />


### Curiosity: Why do we do this?

  : When you write complex code later on, it is beneficial to divide it into zones, such as "Data Loading starts here" or "Graph Plotting starts here." This allows you to isolate and test only the specific Section where an error occurred, rather than having to re-run the entire script every time you make a correction.


# Debug MATLAB Code

If an error occurs while MATLAB is running your program, or if MATLAB detects a significant issue in your code, the status indicator at the top right becomes an error icon. The code issue is also underlined in red.

<img width="688" height="548" alt="Screenshot 2026-05-13 at 3 37 13 pm" src="https://github.com/user-attachments/assets/7f21e743-568e-4aa0-b3ba-dd0abd20d76b" />


## You can view a description of the error by hovering your mouse over the message indicator or the underlined code.

## TASK 1. 

Navigate to the error by clicking the error icon. Then fix the error.

<img width="2072" height="716" alt="Screenshot 2026-05-13 at 3 37 46 pm" src="https://github.com/user-attachments/assets/fb2fc4ba-b57e-4e8f-a433-c299ef5376bf" />

<img width="2076" height="418" alt="Screenshot 2026-05-13 at 3 39 13 pm" src="https://github.com/user-attachments/assets/5f1fc6b7-d69a-47b9-bd68-a03b51e2c13d" />

## Another type of warning signs:

<img width="682" height="766" alt="Screenshot 2026-05-13 at 3 41 04 pm" src="https://github.com/user-attachments/assets/d50fce1a-7a31-47fc-8bce-f7c32de8f099" />

 <img width="2074" height="1036" alt="Screenshot 2026-05-13 at 3 38 03 pm" src="https://github.com/user-attachments/assets/81995142-14ac-4d45-85c0-62aba05af072" />





 # Manually enter array

 ## Array

  * All MATLAB variables are arrays. So, each numeric variable can contain multiple numbers. You can store related data in one variable by using an array. Because arrays are a basic programming tool in the MATLAB language, it's important to get to know them and the terminology used to describe them.

<img width="870" height="598" alt="Screenshot 2026-05-13 at 5 17 46 pm" src="https://github.com/user-attachments/assets/c7702510-09ee-4869-aa3a-9cab22ebd9b8" />


