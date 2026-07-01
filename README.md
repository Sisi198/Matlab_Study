# Matlab_Study

## How to start

### Matlab onramp in Matlab online courses


### When you enter a command without a semicolon at the end, MATLAB displays the result.

EX: 

## TASK 2

Assign the result of 3*5 to a variable named m

>> m = 3*5 

## TASK 3

Enter the command m = m + 1 to see what happens.

<img width="334" height="214" alt="Screenshot 2026-05-10 at 12 16 56 pm" src="https://github.com/user-attachments/assets/7be7a44b-fc14-4a94-b4e1-12d2a058576f" />


## TASK 4

Create a variable named y that has the value of m/2.

<img width="358" height="252" alt="Screenshot 2026-05-10 at 12 17 59 pm" src="https://github.com/user-attachments/assets/b2e98e34-9720-4874-8541-86a7dfcf4119" />


### To add a semicolon to the end of a command so that the result is not displayed. MATLAB still executes the command, and you can see the variable in the Workspace panel.

EX: 

## TASK 5

Enter k = 8 - 2; 

including the semicolon at the end.

**The result won't appear in the Command Window, but you can see the value of k in the Workspace panel.**


<img width="314" height="112" alt="Screenshot 2026-05-10 at 12 30 17 pm" src="https://github.com/user-attachments/assets/f6aa617b-6da5-4d14-bf33-deebc7e54cd6" />


<img width="462" height="368" alt="Screenshot 2026-05-10 at 12 30 57 pm" src="https://github.com/user-attachments/assets/62cfed44-0acb-4c5e-a500-8d0b0c4f0a88" />


### You can recall previous commands by pressing the Up arrow key ↑ on your keyboard. 

### Note. Command Window must be the active window for this keystroke to work.

EX: 

## TASK 6

Press the Up arrow key to return to the command m = 3*5, and before pressing Enter, edit the command to be m = 3*k.


<img width="1012" height="368" alt="Screenshot 2026-05-10 at 12 32 15 pm" src="https://github.com/user-attachments/assets/54f23b7a-2989-4ba0-a01f-d8c1ad99a7c8" />


### When you enter just a variable name at the command prompt, MATLAB displays the current value of that variable.

## TASK 7

In Task 4, you calculated the value of y using the value of m. Was y recalculated when you modified m in Task 6?

Type just the variable name y at the command prompt, and press Enter.

<img width="340" height="250" alt="Screenshot 2026-05-10 at 1 56 53 pm" src="https://github.com/user-attachments/assets/95ad980c-4e4a-4785-a005-3097caf3655f" />


# Name Variables

### You can name your MATLAB variables anything you'd like as long as they start with a letter and contain only letters (A-Z, a-z), numbers, and underscores (_). *(MATLAB variables are also case sensitive)*

EX: 

## TASK 1

Create a variable named A with the value -2.

<img width="336" height="408" alt="Screenshot 2026-05-10 at 2 01 24 pm" src="https://github.com/user-attachments/assets/974828f7-bbf8-447d-a33b-17ad453f308a" />

<img width="470" height="276" alt="Screenshot 2026-05-10 at 2 01 30 pm" src="https://github.com/user-attachments/assets/922968d5-8d07-437e-9442-d1fd3094b1d7" />

## Task 2

Use A and a to calculate 

>> a+A / 2

Store the result in a variable named meanAa.

<img width="520" height="484" alt="Screenshot 2026-05-10 at 2 03 41 pm" src="https://github.com/user-attachments/assets/35e4cd06-31fa-4d8a-9cf8-840787580cb0" />

## Task 3

If you use an invalid variable name, MATLAB displays an error message and a suggested correction. You can use this correction, modify it, or press Esc to delete the suggestion.

<img width="650" height="336" alt="Screenshot 2026-05-10 at 2 06 00 pm" src="https://github.com/user-attachments/assets/8bb18da4-c788-46ec-b16b-8bdc7f037cb0" />


# Save and Load Variables

### You can save variables in your workspace to a MAT-file, a file format specific to MATLAB, by using the save command.

### For example, to save all the variables in the workspace to a MAT-file named filename.mat, use the command:

### >> save filename

## Task 1

<img width="788" height="190" alt="Screenshot 2026-05-10 at 2 07 44 pm" src="https://github.com/user-attachments/assets/831ca738-5bbc-4bda-b2ae-4365a47b9fa7" />


### To remove all the variables from your workspace with the *clear command*.

EX: 
>> clear

### To load variables from a MAT-file, use the load command.

>> load filename

EX: 

## Task 3 

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

## TASK1 

Create a variable named x with a value of π/2.

<img width="580" height="306" alt="Screenshot 2026-05-12 at 9 27 57 pm" src="https://github.com/user-attachments/assets/d2109011-d6a4-43ae-99b9-fa317fac4652" />



MATLAB contains a wide variety of built-in functions, such as abs (absolute value) and eig (eigenvalues).

>> a = sin(-5)

a =  0.9589

Pass inputs to functions by using parentheses, similar to function notation in math.


## TASK 2

Calculate the sine of x by using the sin function. Assign the result to a variable named y.

<img width="470" height="264" alt="Screenshot 2026-05-12 at 9 32 47 pm" src="https://github.com/user-attachments/assets/e03eb4d9-64b0-46b5-a15d-01b95e3cbe1c" />

## TASK 3

Calculate the square root of -9 by using the sqrt function. Assign the result to a variable named z.

<img width="496" height="266" alt="Screenshot 2026-05-12 at 9 33 58 pm" src="https://github.com/user-attachments/assets/b1e87e82-48d6-42d5-996e-72f0d61d83f3" />


Note. the solution contains the imaginary number i : a built-in constant in MATLAB

The Command Window output shows only the first four decimal places. 

You can control the displayed precision with the format function.


## Task 4

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

## Index into Arrays

* To index into a vector, use a single index value. For example, this code returns the 5th element of row or column vector x.
  
    >> y = x(5)

## Task 1.

Create a variable x that contains the value in the 2nd element of the variable v.

>> x = v(2)

<img width="840" height="738" alt="Screenshot 2026-06-16 at 6 26 06 pm" src="https://github.com/user-attachments/assets/1a6b54f7-4fe9-4925-a36e-0d70f048788a" />

* You can use the MATLAB keyword end as an index to reference the last element.

  >> y = x(end)
  
## Task 2. 

Extract the last element of the variable v using the end keyword. Assign this value to a variable named y.

>> y = v(end)

<img width="820" height="830" alt="Screenshot 2026-06-16 at 6 27 16 pm" src="https://github.com/user-attachments/assets/726fb337-942d-4afb-9588-09df92dada60" />

* You can use arithmetic with the keyword end.

* For example:
  >> y = x(end-2)

## Task 3. 

Create a variable z that contains the value in the second-to-last (end-1) element of v.

>> z = v(end-1)

<img width="830" height="914" alt="Screenshot 2026-06-16 at 6 28 17 pm" src="https://github.com/user-attachments/assets/5afb6eb9-af73-40c5-a8de-675708de8b50" />

* You can extract values from a matrix using row-column indexing.

  >> y = A(5,7)

* This syntax extracts the value in the 5th row and 7th column of A and assigns the result to the variable y.

## Task 4. 

Create a variable a that contains the value in the 6th row and 3rd column of the variable data.

>> a = data(6,3)

<img width="828" height="790" alt="Screenshot 2026-06-16 at 6 29 42 pm" src="https://github.com/user-attachments/assets/8acdd9de-81c4-4d40-bd32-5d15d8f1db6c" />


* You can use end as either a row or column index to reference the last row or the last column, respectively.

  >> y = A(end,2)
  
## Task 5. 

Extract the value in the last row and 3rd column of the variable data. Assign this value to a variable named b.

>> b = data(end,3)

<img width="786" height="844" alt="Screenshot 2026-06-16 at 6 31 42 pm" src="https://github.com/user-attachments/assets/c970ccb8-cc30-4b2e-92e6-c74b6839d0f4" />


* If you use only one index with a matrix, MATLAB traverses down each column in order. For example, this code returns the value 6.

  >> A = [5 6; 7 8]
  >> A(3)
  
* Core Concept: Linear Indexing in MATLAB
   * The sorting rule it uses for this line is called Column-major order. This means MATLAB lines up the entirety of Column 1 first, and then appends Column 2 right underneath it.
  1. The Structure of Matrix A:
      * When you define A = [5 6; 7 8], MATLAB builds a $2 \times 2$ matrix that looks like this:
        <img width="350" height="196" alt="Screenshot 2026-06-16 at 6 37 01 pm" src="https://github.com/user-attachments/assets/73f522c9-2cb2-4754-b98f-362279d8288c" />
      * Column 1: 5, 7 & Column 2: 6, 8

  2. How MATLAB Flattens the Grid in Memory

      * If you pass only a single index like A(3) instead of using coordinate subscripts like A(row, col), MATLAB searches for the number based on its linear position in memory.
    
      * It counts the positions by moving downwards from top to bottom through each column:
      
        1. 1st position: 5 (Row 1, Column 1)
        2. 2nd position: 7 (Row 2, Column 1 $\rightarrow$ moving down the column)
        3. 3rd position: 6 (Row 1, Column 2 $\rightarrow$ Column 1 is finished, moving to the top of the next column)
        4. 4th position: 8 (Row 2, Column 2)
        
      * When completely flattened into a linear array, the sequence becomes: [5, 7, 6, 8].
    
  3. Why does A(3) return 6?

   * Because MATLAB scans the flattened sequence and pulls the value sitting at the exact 3rd position:

     * A(1) is 5
     * A(2) is 7
     * A(3) is 6
     * A(4) is 8


## Task 6.

Using one index, try extracting the eighth element of data. You can also use a variable as an index. Try creating a variable idx with the value 8 and using idx as the index to data.


>> idx = 8;
>> result = data(idx)

<img width="396" height="48" alt="Screenshot 2026-06-17 at 5 34 22 pm" src="https://github.com/user-attachments/assets/af2c1fac-1d0b-444d-926e-28e7f43d7e57" />

___________________________ Another way:

>> data(8)

<img width="670" height="134" alt="Screenshot 2026-06-16 at 6 41 24 pm" src="https://github.com/user-attachments/assets/472d9cef-64c0-412a-a800-54a86ef5f281" />


The reason why idx 8 is 0.5300:

<img width="788" height="336" alt="Screenshot 2026-06-16 at 6 41 15 pm" src="https://github.com/user-attachments/assets/6248f384-60c0-4a59-8b22-fbeb03086ebf" />


## Extract Multiple Elements

* When used as an index, the colon operator (:) specifies all the elements in that dimension. For example, this code creates a column vector containing all the elements from the first column of A.
    
  >> x = A(:,1)

## Task 1.
Create a column vector named density that contains all the elements from the 2nd column of the matrix named data.

>> density = data(:, 2)

<img width="2088" height="1334" alt="Screenshot 2026-06-17 at 5 39 58 pm" src="https://github.com/user-attachments/assets/bbdae345-c411-4a34-b86e-53ac07f6b74c" />

* You can use the colon operator to specify a range of values. This code creates a matrix containing the first, second, and third rows of the matrix A.

   >> x = A(1:3,:)

## Task 2.
Create a variable volumes that contains the last two columns of data. You can see the size of data in the output pane to the right of your screen.

>> volumes = data(:,3:4)
_________________________ Another way:
>> volumes = data(:,end-1)

<img width="2070" height="1076" alt="Screenshot 2026-06-17 at 5 41 54 pm" src="https://github.com/user-attachments/assets/0c042e00-a254-4bf8-ad35-ee23c8d4665a" />
<img width="2098" height="1066" alt="Screenshot 2026-06-17 at 5 43 17 pm" src="https://github.com/user-attachments/assets/de2fc5f7-3717-41c6-b0c9-ea09d200698f" />


* You can also extract multiple elements from a vector. Recall that for indexing into vectors, you only provide one input. For example, this code returns a subset of vector v containing the elements from index 3 to the end.

  >> x = v(3:end)

## Task 3.

Create a vector named p containing the 2nd through 5th elements of density.

>> p = density(2:5)

<img width="2126" height="1302" alt="Screenshot 2026-06-17 at 5 45 11 pm" src="https://github.com/user-attachments/assets/ddbc37c7-f5b1-4404-9c4c-370cddb0fff6" />


## Task 4.

Indices can be nonconsecutive numbers. For example, you can use [1 3 6] as an index to extract the first, third, and sixth elements of density: 


>> density([1 3 6])

<img width="2098" height="1376" alt="Screenshot 2026-06-17 at 5 46 33 pm" src="https://github.com/user-attachments/assets/6a77a336-c13c-488b-97c7-6432b06822b7" />


# Change Values in Arrays

* If you know the position of an element, you can change its value by combining indexing with assignment.

* For example, to change the third element of x to 1, you reference the third element with x(3) and then use the assignment operator = to assign the value 1 to that element.
  
  >> x(3) = 1

## Task 1.

Change the first element of v2 from NaN to 0.5.

>> v2(1) = 0.5

<img width="2122" height="1340" alt="Screenshot 2026-06-17 at 6 59 26 pm" src="https://github.com/user-attachments/assets/243bf2a7-4408-4dcb-b278-7973380ce443" />

* You can also use indexing to change the elements in a matrix. Remember to specify the row and column when indexing into a matrix.
  
  >> A(3,2) = 1
  
## Task 2. 

Change the element in the first row and last column of data to 0.5.

>> data(1,end) = 0.5

<img width="2092" height="1400" alt="Screenshot 2026-06-17 at 7 01 00 pm" src="https://github.com/user-attachments/assets/5022faf7-7813-4225-8bb1-6e5a42d2afd1" />


* You can combine indexing with assignment to change array elements to other elements. For example, this code changes the value of x(1) to x(2).
  
x(1) = x(2)

## Task 3. 

Try changing the first column of data to the second column of data.

>> data(1) = data(2)

<img width="818" height="504" alt="Screenshot 2026-06-24 at 5 06 24 pm" src="https://github.com/user-attachments/assets/549c4ced-01c3-4217-b183-575c245a3a9a" />


# Perform Array Operations on Vectors

MATLAB is designed to work naturally with arrays. For example, you can add a scalar value to all the elements of an array.
x = [1 2 3];
y = x + 2
y = 
     3     4     5


## Task 1. 

Add 1 to each element of v1 and store the result in a variable named r.

>> r = v1 + 1

<img width="2078" height="766" alt="Screenshot 2026-06-24 at 5 09 27 pm" src="https://github.com/user-attachments/assets/edb6a914-d8d8-44d9-a787-3698be2ad4a4" />

* You can add any two arrays of the same size.

  z = x + y

## Task 2.

Create a vector vs that is the sum of the vectors v1 and v2.

>> vs = v1 + v2

<img width="2060" height="360" alt="Screenshot 2026-06-29 at 6 30 13 pm" src="https://github.com/user-attachments/assets/c12ad82a-5436-43db-aec9-4e9ffada5e95" />


* You can multiply or divide all the elements of an array by a scalar.

>> z = 2*x
>> y = x/3


## Task 3. 

Create a variable va that contains the vector vs divided by 2.

>> va = vs/2

<img width="2134" height="550" alt="Screenshot 2026-06-29 at 6 30 54 pm" src="https://github.com/user-attachments/assets/e195472d-4947-469b-afce-4984e0a9a245" />


* You can apply basic statistical functions in MATLAB to a vector to produce a single output.

* For example, the maximum value of a vector can be determined using the max function.

   >> xMax = max(x)
   
## Task 4. Create a variable vm that contains the maximum of the va vector.

>> vm = max(va)

<img width="2100" height="298" alt="Screenshot 2026-06-29 at 6 32 18 pm" src="https://github.com/user-attachments/assets/df75117c-2ea5-456a-a461-fd1b83780430" />


* MATLAB has functions that perform mathematical operations on an entire array of values in a single command.

* For example, you can find the square root of each element in the array x with this syntax.
  
  >> xSqrt = sqrt(x)
  
## Task 5. Using the round function, create a variable named vr that contains the rounded elements of va.

>> vr = round(va)

<img width="2062" height="492" alt="Screenshot 2026-06-29 at 6 34 57 pm" src="https://github.com/user-attachments/assets/a6a4ca72-57ef-4040-9375-fc8d786e5e8a" />


* The "*" operator performs matrix multiplication.

* So, if you use "*" to multiply two equally sized vectors, you get an error message because the inner dimensions do not agree.

  >> z = [3 4] * [10 20]
  >> Error using  *
  >> Incorrect dimensions for matrix multiplication. 

* The ".*" operator performs element-wise multiplication by multiplying the corresponding elements of two equally sized arrays.

  >> z = [3 4] .* [10 20]
  >> z = 
      30    80
  
## Task 6. Create a variable named mass that contains the element-wise product of density and va.

>> mass = [density] .* [va]

<img width="2032" height="410" alt="Screenshot 2026-06-29 at 6 37 52 pm" src="https://github.com/user-attachments/assets/7613b18e-6267-4b57-8c2b-a0c0868df92c" />


## Task 7. There are other compatible sizes. For example, try: x = [1 2; 3 4; 5 6; 7 8].*[1;2;3;4] What size is x?

1. Verifying the Dimensions of the Operands. Standard matrix operations require strict dimension matching. 

  However, if one of the arrays contains a dimension size of 1, MATLAB applies flexible alignment rules:
  
    First array: [1 2; 3 4; 5 6; 7 8] $\rightarrow$ Dimensions: 4 x 2
    Second array: [1; 2; 3; 4] $\rightarrow$ Dimensions: 4 x 1

2. Under the Hood: How MATLAB Handles Broadcasting. The ".*" operator denotes element-wise multiplication. 

  To force the 4 x 1 column vector to match the dimensions of the leading 4 x 2 matrix, MATLAB automatically duplicates the existing column along the horizontal axis to expand its footprint.
  
  In practice, the trailing vector [1; 2; 3; 4] is internally projected into a 4 x 2 grid like this:

     <img width="828" height="324" alt="Screenshot 2026-06-30 at 5 26 32 pm" src="https://github.com/user-attachments/assets/995c04f5-4409-4ff4-ad8a-9c6d3e860c21" />

3. The Actual Element-by-Element Computation

   Once the dimensions are perfectly matched, MATLAB multiplies the overlapping coordinates element by element:

     <img width="1184" height="362" alt="Screenshot 2026-06-30 at 5 27 15 pm" src="https://github.com/user-attachments/assets/7e0ca179-b907-4503-852c-7e9119014d0d" />

   This yields the following final output for matrix x:

      <img width="428" height="244" alt="Screenshot 2026-06-30 at 5 27 53 pm" src="https://github.com/user-attachments/assets/3c590c16-f400-4adf-9479-066a25701fe8" />

### $\rightarrow$ Counting the rows and columns of this final matrix confirms that the output size is 4 x 2.


# Function calls

## Request Multiple Outputs in Function Calls

* You can apply the size function to a vector or matrix to produce a single output variable containing the array size in a two-element row vector.
* The first element is the number of rows and the second element is the number of columns.

  >> s = size(x)
  
## Task 1. Create a variable named dsize containing the size of the data variable.

  >> dsize = size(data)

  <img width="2000" height="740" alt="Screenshot 2026-06-30 at 7 50 39 pm" src="https://github.com/user-attachments/assets/01a5d214-c36f-46e0-9970-2476c25e9cbb" />

* You can also request two output variables from the size function. In this case, each variable contains the size of one of the dimensions of the input array. Use square brackets ([ ]) to request more than one output.

  >> [xrow,xcol] = size(x)

  
## Task 2. Create the variables dr and dc that respectively contain the number of rows and columns of the variable data.

  >> [dr,dc] = size(data)

  <img width="2054" height="730" alt="Screenshot 2026-06-30 at 7 52 28 pm" src="https://github.com/user-attachments/assets/9c5d3b27-991e-4cdf-b0f5-a86db80ea534" />

* You can find the maximum value of a vector and its corresponding index value using the max function. The first output from the max function is the maximum value of the input vector. When called with two outputs, the second output is the index value.
  
  >> [xMax,idx] = max(x)

## Task 3. Create the variables vMax and ivMax containing the maximum value of the v2 vector and the corresponding index value, respectively.

  >> [vMax, ivMax] = max(v2)
  
  <img width="2054" height="854" alt="Screenshot 2026-06-30 at 7 55 51 pm" src="https://github.com/user-attachments/assets/b1da072e-65b6-4f8f-abe7-01d8aaf39a9c" />

* If you need only the second output from a function, you can ignore the first output by using a tilde (~) in its place.

* For example, you can just get the number of columns in a matrix:

  >> [~,xcol] = size(x)

  <img width="2018" height="1062" alt="Screenshot 2026-06-30 at 7 57 54 pm" src="https://github.com/user-attachments/assets/feaadd72-b3c4-4f62-bc01-449833db2b29" />

# Documentation

## Use MATLAB Documentation

* The MATLAB documentation contains examples and information that can help you when working on your own problems.

## Task 1. Use the documentation for randi to help complete this task.

Create a matrix named x that:

Contains random integers in the range from 1 to 20

Has 5 rows

Has 7 columns

  >> x = randi(20, 5, 7)

<img width="2094" height="582" alt="Screenshot 2026-06-30 at 8 03 21 pm" src="https://github.com/user-attachments/assets/36f01cde-6b90-48f7-8b8e-39f021627e4f" />

* You can also open the documentation using the doc function. If you know the name of the function and want more information about it, you can use this command:

  >> doc randi

* However, if you don't know the name of the function, you can search the documentation using phrases. Try searching the documentation for a function that creates normally distributed numbers (instead of uniformly distributed numbers) using:

  >> doc normally distributed numbers

# Plots

* You can plot two vectors of the same length against each other using the plot function.

  >> plot(x,y)

## Task 1. Create a plot with sample on the x-axis and mass1 on the y-axis.

  >> plot(sample, mass1)

  <img width="2094" height="1180" alt="Screenshot 2026-06-30 at 8 10 21 pm" src="https://github.com/user-attachments/assets/c5a91bc3-eb2a-4380-8002-93fc09bfbb08" />

* You can specify the colour, line style, and marker of a plot by using different symbols in double quotes as another input to the plot function.

  >> plot(x,y,"r--o")

* The command plots a red (r) dashed (--) line with circle (o) markers.


<img width="2002" height="658" alt="Screenshot 2026-06-30 at 8 11 46 pm" src="https://github.com/user-attachments/assets/936ea995-2974-4863-a689-86b8a522f1d0" />
<img width="1968" height="1164" alt="Screenshot 2026-06-30 at 8 11 55 pm" src="https://github.com/user-attachments/assets/b796eb5f-4abe-4c2f-a453-26040da75de3" />
<img width="1972" height="812" alt="Screenshot 2026-06-30 at 8 12 01 pm" src="https://github.com/user-attachments/assets/878387fd-97eb-4f40-a79e-d20b178019f0" />



## Task 2. Plot mass2 (y-axis) against sample (x-axis). Use red (r) star (*) markers and no line in your plot.

First attempt:

>> plot(sample, mass2, "r--*")

<img width="2780" height="1238" alt="Screenshot 2026-07-01 at 5 28 38 pm" src="https://github.com/user-attachments/assets/d1553d0e-4151-4626-9819-8a7710c6c914" />

$\rightarrow$ error occurs, reading the instruction again; find out it says, "no line", change the input


Second attempt:

>> plot(sample, mass2, "r*")

<img width="2786" height="1298" alt="Screenshot 2026-07-01 at 5 28 53 pm" src="https://github.com/user-attachments/assets/a1a930e5-f911-4b90-8b23-7571c59ae5c1" />


* Notice that each plot command created a separate plot. You can plot one line on top of another in the same axes by using the hold on command.
  
  >> plot(x1,y1)
  >> hold on
  >> plot(x2,y2)
  
## Task 3. Enter the hold on command. Then plot mass1 (y-axis) against sample (x-axis) with magenta (m) square (s) markers and no line.
  
  >> plot(sample, mass1)
  >> hold on
  >> plot(sample, mass1, "ms")


  <img width="2030" height="654" alt="Screenshot 2026-07-01 at 5 32 32 pm" src="https://github.com/user-attachments/assets/2faeb29c-0944-4f26-ae8e-50a51585dbc0" />
  <img width="2048" height="656" alt="Screenshot 2026-07-01 at 5 32 49 pm" src="https://github.com/user-attachments/assets/66b842c9-1363-490c-9e8e-12f38682416c" />


### $\rightarrow$ Q. How the Graphs Overlap (The Layer Concept): Inside MATLAB, the rendering is structured as three distinct sheets stacked on top of one another:
  
  * Layer 1: plot(sample, mass1) $\rightarrow$ Draws the initial blue line.
  * Layer 2: hold on $\rightarrow$ Freezes the current canvas (Layer 1) and places a transparent sheet directly over it.
  * Layer 3: plot(sample, mass1, "ms") $\rightarrow$ Draws only the magenta square markers on that new transparent sheet.

* As a result, because these sheets are stacked, you see the magenta squares sitting perfectly along the blue line. If you hadn't used hold on, the moment Layer 3 was executed, Layer 1 (the blue line) would have been thrown into the trash, leaving only the magenta squares behind on a blank canvas.

$\rightarrow$  "the modified elements were newly added and superimposed on top"

----------------------------------
* While the hold state is on, plots continue to appear on the same axes. To return to the default plot behaviour, where each plot appears on its own axes, enter hold off.


## Task 4. Enter the hold off command.

  >> hold off


* When you plot a single vector by itself, MATLAB uses the vector values as the y-axis data and sets the x-axis data to the range of 1 to n (the number of elements in the vector).

  >> plot(y)


## TASK 5. Plot the vector v1.

  >> plot(v1)

  <img width="840" height="640" alt="Screenshot 2026-07-01 at 5 58 39 pm" src="https://github.com/user-attachments/assets/04ed0c15-5443-4ea6-ba04-1806d4a0115c" />


* When you use the plot function, you can optionally set properties using one or more name-value arguments, which consist of an argument name and an associated value. For example, this command plots a heavy line.

  >> plot(y,LineWidth=5)

## Task 6. Plot v1 with a line width of 3.

  >> plot(v1, LineWidth=3)

    <img width="2052" height="660" alt="Screenshot 2026-07-01 at 5 59 51 pm" src="https://github.com/user-attachments/assets/25831496-0d8e-4c20-90fc-20d7bfddd27b" />

* You can provide name-value arguments to the plot function after the line specification.

  >> plot(x,y,"ro-",LineWidth=5)
  
## Task 7. Plot v1 (y-axis) against sample (x-axis) with red (r) circle (o) markers and a solid line (-). Use a line width of 4.

  >> plot(sample, v1, "ro-", LineWidth=4)

  <img width="824" height="606" alt="Screenshot 2026-07-01 at 6 02 56 pm" src="https://github.com/user-attachments/assets/33ef097f-9647-44bb-b0e9-65006c09b196" />

# Annotate Plots

* You can add labels to plots using plot annotation functions, such as title. The input to these functions is text. Text in MATLAB is enclosed in double quotes (").

  >> title("Plot Title")
  
## Task 1. Add the title "Sample Mass" to the existing plot.

  >> title("Sample Mass")

  <img width="2000" height="578" alt="Screenshot 2026-07-01 at 6 29 18 pm" src="https://github.com/user-attachments/assets/5b8c89e0-b363-4147-be63-3b90fa4e6eee" />



* You can add labels to your axes using the xlabel and ylabel functions.

  >> ylabel("Y-Axis Label")

## Task 2. Add the y-axis label "Mass (g)".

  >> ylabel("Mass (g)")
  
  <img width="848" height="790" alt="Screenshot 2026-07-01 at 6 30 47 pm" src="https://github.com/user-attachments/assets/e5b790ae-479c-43fc-8466-e8c4a766bd3d" />


* You can add a legend to your plot using the legend function.

  >> legend("a","b","c")

## Task 3. Create a legend with the labels "Exp A" and "Exp B", in that order.

  >> legend("Exp A", "Exp B")

  <img width="854" height="742" alt="Screenshot 2026-07-01 at 6 37 43 pm" src="https://github.com/user-attachments/assets/cbcd3b09-5371-49a3-966f-7d3a847ae72e" />

