# You need to do 2 things here.

1. creating a python file (my code is compatible with python 3.6)
2. schedule a command in windows scheduler to run this python file at your defined time 

For scheduling the task (here python job) in windows...
open windows -> type scheduler - > you should able to see "Task Scheduler" 
click on task scheduler library
rightlick on this
create new task
a pop-up shows
in general tab - give a name and select "run only when user logged on "
Trigger tab - New- > create your schedule as to tell windows scheduler when to trigger this job..
in actions tab -  dropdown select - start a program and  in the script field : give location of where python.exe is present in your machine..
example in my case: "C:\Users\abc\Desktop\python exp\python.exe" 
 in the same tab, below the script field, you need to provide the arguments needed fro this program
 in our case the program is python and the argument should be like the path where your actual python code is 
 
 in my case : "C:\Users\abc\Desktop\python exp\gold_rate.py"
 Note: if your folder name has spaces in between, then you are prone to get errors, as the string looks split.. so always give path in double quotes.
 
 
 Thats it!! you are all set to wait and see if your code gets kicked off based on what time you set!!!
