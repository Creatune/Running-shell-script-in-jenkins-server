# Running-shell-script-in-jenkins-server
This is a blog on how to run a simple shell script that performs the grub command on jenkins server
First of all run jenkins server.
Create a job and name it. The job should be in freestyle mode only.
Open a .txt file and type in some sentences with the word 'status' in them and some sentences without the word 'status' in them.
Now, open a .sh file and type whatever is provided in the given repository, except instead of my directories in grep, give your own directory path.
Go to the job that you created earlier in jenkins. Click the configure button on the left hand side of the project dashboard.
Scroll down to the build option and select 'execute shell' in the drop down menu that appears.
Now, a huge command box should appear. In this box, just paste whatever you have written in the .sh file. Save these changes.
Now, you will automatically be taken back to the project dashboard. Click the build option just above the configure option. After a few seconds, you will see that a build histroy is created just under all the options on the left hand side.
In that build history you will see your project's build represented as a coloured ball. If the ball is blue, your project is a success! If it is red, then there is an error in executing the shell script.
To avoid that, defining your paths clearly will help. If there is a permission denial, then use the command: chmod 755 <.sh file>
After that run the shell script.
Thus, we have successfully run a shell script in a jenkins server :)
