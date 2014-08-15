Patricks-MacBook-Pro:learn_command_line_exercises patrickcarter$ cd chapter_10
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cd .
Patricks-MacBook-Pro:chapter_10 patrickcarter$ mine .
Patricks-MacBook-Pro:chapter_10 patrickcarter$ touch readme.md
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cd ..
Patricks-MacBook-Pro:learn_command_line_exercises patrickcarter$ cd chapter_10
Patricks-MacBook-Pro:chapter_10 patrickcarter$ mkdir tmp
Patricks-MacBook-Pro:chapter_10 patrickcarter$ touch iamcool.txt neat.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
iamcool.txt	neat.txt	readme.md	tmp
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp awesome.txt iamcool.txt 
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
iamcool.txt	neat.txt	readme.md	tmp
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp neat.txt awesome.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt	iamcool.txt	neat.txt	readme.md	tmp
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cd awesome.txt thefourthfile.txt
bash: cd: awesome.txt: Not a directory
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp awesome.txt thefourthfile.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		neat.txt		thefourthfile.txt
iamcool.txt		readme.md		tmp
Patricks-MacBook-Pro:chapter_10 patrickcarter$ mkdir something
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp awesome.txt something/
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		readme.md		tmp
iamcool.txt		something
neat.txt		thefourthfile.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r something newplace
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls newplace/
awesome.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$


Do More
Use the cp -r command to copy more directories with files in them.
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r awesome.txt newplace
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		newplace		thefourthfile.txt
iamcool.txt		readme.md		tmp
neat.txt		something

Copy a file to your home directory or desktop.
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r neat.txt desktop
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		neat.txt		something
desktop			newplace		thefourthfile.txt
iamcool.txt		readme.md		tmp

Find these files in your graphical user interface and open them in a text editor.

Notice how sometimes I put a / (slash) at the end of a directory? 
That makes sure the file is really a directory, 
so if the directory doesn't exist I'll get an error.

Alternative "english" ways of asking you to copy a file:

Can you copy the foo.txt file to slash temp?  (Create foo.txt first...)
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r foo.txt tmp/
cp: foo.txt: No such file or directory
Patricks-MacBook-Pro:chapter_10 patrickcarter$ touch foo.txt
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		neat.txt		thefourthfile.txt
desktop			newplace		tmp
foo.txt			readme.md
iamcool.txt		something
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cd -r foo.txt tmp/
bash: cd: -r: invalid option
cd: usage: cd [-L|-P] [dir]
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r foo.txt tmp/
Patricks-MacBook-Pro:chapter_10 patrickcarter$ ls
awesome.txt		neat.txt		thefourthfile.txt
desktop			newplace		tmp
foo.txt			readme.md
iamcool.txt		something
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cd tmp
Patricks-MacBook-Pro:tmp patrickcarter$ ls
foo.txt

Can you copy .bash_profile in your home directory to the current directory?
Patricks-MacBook-Pro:chapter_10 patrickcarter$ cp -r .bash_profile tmp/
cp: .bash_profile: No such file or directory
