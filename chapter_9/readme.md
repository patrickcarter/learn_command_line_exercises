Patricks-MacBook-Pro:learn_command_line_exercises patrickcarter$ mkdir tmp
Patricks-MacBook-Pro:learn_command_line_exercises patrickcarter$ cd tmp
Patricks-MacBook-Pro:tmp patrickcarter$ touch iamcool.txt
Patricks-MacBook-Pro:tmp patrickcarter$ ls
iamcool.txt

DO MORE:
Unix: Make a directory, change to it, 
mkdir test
cd test

and then make a file in it.
touch test.txt

Then change one level up and run the rmdir command in this directory.
Patricks-MacBook-Pro:tmp patrickcarter$ rmdir test
rmdir: test: Directory not empty

You should get an error. Try to understand why you got this error.
Cant delete a dir that is not empty

Alternative "english" ways of asking you to create a file:

Can you touch blah.txt?
Yes I can, but if blah.txt gets pissed I am blaming you.
Patricks-MacBook-Pro:tmp patrickcarter$ touch blah.txt
Patricks-MacBook-Pro:tmp patrickcarter$ ls
blah.txt	iamcool.txt	test

Let's create foo.txt.
Patricks-MacBook-Pro:tmp patrickcarter$ touch foo.txt
Patricks-MacBook-Pro:tmp patrickcarter$ ls
blah.txt	foo.txt		iamcool.txt	test
