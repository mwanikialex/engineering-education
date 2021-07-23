    • ## overview
In Linux operating systems files and applications are installed in many ways. Some applications come in form of Debian packages with the extension (<package name>.deb) ,Rpm packages with the extension (<package name>.rpm) and lastly tar.gz files with the extension (<package name.tar.gz>).
    • ##prerequisites

    • 1.Linux operating system
    • 2.Archive manager —- comes pre-installed in the operating system no need to install it
    • 3.chrome web browser
    • 4.Linux terminal
    • 5.Know basic Linux terminal commands like ls (to show the contents of the specified folder), Cd(to move the terminal location to specifies point), chmod(makes the files executable and to be  installable ) 
    • 6.wine is used to run windows programs in Linux systems.

    • ##tar.gz application
In this section, we look at tar.gz packages and how we install them on Linux operating systems. Some packages one will download when using Linux in his/her lifetime with the OS will come in form of tar.gz binaries. They are sometimes called tarball files.
 Such binaries come as compressed files with information or files inside them. The reason behind this analogy is to save space mostly and they become easy to download and save on one's computer. Tar .gz files also may contain passwords i.e they may be locked by the user and may ask for password privileges to be used. 
    • ##Installation
First off we download the tar.gz binary or package we want to install. In this example, I will use a package called Waon player tar.gz. Go to your chrome web browser and choose your preferred search engine like Google and in the address search bar type Waon player download or paste this link on the search bar [waon download](http://kichiki.github.io/waon/dist/index.html). They can the extension (.targz) or (.tgz) or (.tar.bz2) or (.tbz2).
![image title](/tar-gz-files/chrome.png)

Once you download the package it normally appears in your download folder. Minimize chrome window and move to file manager or files according to your Linux distro distribution. Open the terminal by pressing Control+Alt+T at the same time.

![image title](/tar-gz-files/terminal.png)

Inside the terminal  type the following command
'code' $  cd Downloads 
to move the terminal location to the downloads sections. It should look like this

![image title](/tar-gz-files/downloads.png)

 Then type
$ 'code' ls
to check the location of the file you downloaded. Then type 
'code' $ tar xvzf <Package name>.tar.x.z in our case we type
'code' $  tar xvzf waon-0.9.tar.gz to extract the files 

![image title](/tar-gz-files/extract.png)

.They appear in the same place as the tarball. Type the ‘ls’ command to check.


Now we place the terminal in the extracted files folder by typing 
'code' $ cd waon-0.9

![image title](/tar-gz-files/waon.png)


Commonly, the tar.gz package or binary one downloads contains a file/files with the specifications to execute the program. The package we will use today contains a file named ‘INSTALL’ with the instructions on the installation process for the package.
Try and find a configuration script. This file checks if your system has all the requirements required for the building or may contain the requirements text. If you find the required  script/file you can execute it as follows
'code' $ ./configure.
      In our case, we will use the ‘make’ command to configure the makefile. gwaon file. In the terminal type
'code' $ make -f Makefile. gwaon

![image title](/tar-gz-files/makefile.png)


AS seen below ours contains the INSTALL  file in the extracted folder. After this process, we get an executable file in our directory.


Now we execute our program in the terminal to install it using the executable file we created from the above step above. This file named waon.1 is executable. For example a file in Windows operating systems with the extension of  (.exe) which in that scenario it will executable and can be easily installed. Here our file (waon.1) is executable.

![image title](/tar-gz-files/made.png)

Now I must execute my program. In most cases, the installation of the program on your computer must use the 'make' install command in the Linux terminal pointing to the source. For this process configure the tarball or tar.gz file with this command
'code'$ sudo ./ configure

![image title](/tar-gz-files/execute.png)

This command should be used after extracting the files and the terminal should be directed in the executable file of your application. After this type
'code' $ make <executable file>

The Linux OS ‘make’ command is used to build and store groups of files and software from the source code you have downloaded from. It helps computer engineers to configure and run much software from the terminal.

After this type the command 
'code' $sudo make install 

‘sudo make’ install command lets you install the files in directories that are read-only to you as the computer owner and such. Enter your password in the terminal and hit enter.
For my application, the last command isn't necessary because the application once made using the make command it is installed.

 This process allows you to install your application. At the most time after installation one is needed to reboot his/her computer for most of the software installation process to complete.













 











 












