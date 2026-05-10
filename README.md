# Matlab_Study

Matlab study


## How to start

### Matlab onramp in Matlab online courses


When you enter a command without a semicolon at the end, MATLAB displays the result.

TASK 2

Assign the result of 3*5 to a variable named m, as shown.

m = 3*5 

TASK 3

Enter the command m = m + 1 to see what happens.

<img width="334" height="214" alt="Screenshot 2026-05-10 at 12 16 56 pm" src="https://github.com/user-attachments/assets/7be7a44b-fc14-4a94-b4e1-12d2a058576f" />


TASK 4

Create a variable named y that has the value of m/2.

<img width="358" height="252" alt="Screenshot 2026-05-10 at 12 17 59 pm" src="https://github.com/user-attachments/assets/b2e98e34-9720-4874-8541-86a7dfcf4119" />


Optionally, you can add a semicolon to the end of a command so that the result is not displayed. MATLAB still executes the command, and you can see the variable in the Workspace panel.

TASK 5

Enter k = 8 - 2; 

including the semicolon at the end.

The result won't appear in the Command Window, but you can see the value of k in the Workspace panel.


<img width="314" height="112" alt="Screenshot 2026-05-10 at 12 30 17 pm" src="https://github.com/user-attachments/assets/f6aa617b-6da5-4d14-bf33-deebc7e54cd6" />


<img width="462" height="368" alt="Screenshot 2026-05-10 at 12 30 57 pm" src="https://github.com/user-attachments/assets/62cfed44-0acb-4c5e-a500-8d0b0c4f0a88" />


You can recall previous commands by pressing the Up arrow key ↑ on your keyboard. Note that the Command Window must be the active window for this keystroke to work.

TASK 6

Press the Up arrow key to return to the command m = 3*5, and before pressing Enter, edit the command to be m = 3*k.


<img width="1012" height="368" alt="Screenshot 2026-05-10 at 12 32 15 pm" src="https://github.com/user-attachments/assets/54f23b7a-2989-4ba0-a01f-d8c1ad99a7c8" />


When you enter just a variable name at the command prompt, MATLAB displays the current value of that variable.

TASK 7

In Task 4, you calculated the value of y using the value of m. Was y recalculated when you modified m in Task 6?

Type just the variable name y at the command prompt, and press Enter.

<img width="340" height="250" alt="Screenshot 2026-05-10 at 1 56 53 pm" src="https://github.com/user-attachments/assets/95ad980c-4e4a-4785-a005-3097caf3655f" />


# Name Variables
You can name your MATLAB variables anything you'd like as long as they start with a letter and contain only letters (A-Z, a-z), numbers, and underscores (_). *(MATLAB variables are also case sensitive)*

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

Task 1

You can save variables in your workspace to a MAT-file, a file format specific to MATLAB, by using the save command.

For example, to save all the variables in the workspace to a MAT-file named filename.mat, use the command:
>> save filename

<img width="788" height="190" alt="Screenshot 2026-05-10 at 2 07 44 pm" src="https://github.com/user-attachments/assets/831ca738-5bbc-4bda-b2ae-4365a47b9fa7" />

Task 2

To remove all the variables from your workspace with the *clear command*.

EX: 
>> clear


