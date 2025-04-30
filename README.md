# linux_server

> # INTRODUCTION TO LINUX



* In the dynomic landscape of technology, mastering the fundamentals is essential for anyone aspiring to excel in fields such as DevOps, Cloud Computing, Software Development, Cybersecurity, Data Analysis/Science, Al, and QA Testing. This project is designed to equip you with a solid foundation in Linux. Understanding the tech from the basics lays the groundwork fo success in various tech-centric careers. 


 > # WHAT IS LINUX?
* Linux is a free, open-source operating system similar to Windows or macOS, but it's more widel used for servers and supercomputers. It's known for its stability, security, and flexibility, allowing users to modify and distribute their versions. Linux runs on a wide range of devices, from desktops to smartphones, and powers much of the internet's infrastructure. It's supported by a global community of developers who contribute to its many distributions, each tailored for specific needs or preferences.

> # LINUX DISTRIBUTION
 * Linux distributions, often referred to as 'distros', are different flavours of the Linux operating systems built using the Linux kernel. These distros package the Linux kernel with a range of software, libraries, and tools to provide a functional computing environment. They offer different configurations, desktop environments, package managers, and software repositories, and ther they are branded. Some of the Linux distributions are;
Ubuntu: Ubuntu is one of the most widely recognized Linux distributions, known for its user-friendliness and ease of installation. It's an excellent choice for those new to Linux, as well as fo everyday desktop computing. Ubuntu has server editions for web hosting and cloud deployments.


> # INSTALLATION AND INITIAL SETUP
 * In this section, we will create a server in the cloud, and gain access to it from our local environment. When we say Local environment" we are referring to your laptop, or the desktop PC you are using to work or learn. Which would have either Windows, or Mac operating system in most cases. Then you will connect to that server in the cloud, remotely straight from your laptop.


 * We will use AWS, a public cloud provider to create the server in the cloud. For now, do not worr about trying to learn AWS because there is a complete course on that, and plenty of projects ahead that focuses on that.
Right now, all you need to know is that AWS can provide us with a free virtual server called EC2
Elastic Compute Cloud.
Let us create an EC2 instance. i.e a Linux Server
You can either Watch the videos below to get yourself set up.
AWS account setup and Provisioning an Ubuntu Server
Connecting to your EC2 Instance
Or follow the guideline below.

i. Register a new AWS account following this instruction.

ii. Sign in to your AWS account
![](/Images/sign%20in%20aws.png)


iii. On the top left select services and search for Elastic Cloud Compute (EC2).
![](/Images/select%20%20ec2.png)


iV. From the menu on the left side, select instances.
![](/Images/launch%20instance.png)

* The following images are direction and guideline given so it can be followed directly 

1. I was told to name the tag with "LINUX_SERVER"
![](/Images/launch%20instance.png)


2. I was told to name the prem as "key" which made accessing it easy 
![](/Images/key%20prem.png)

3. I was also told to to increase the internal memory fro 8gb to 15 gb


> # CLIENT TOOL

To install
If you are on windows, you will need to have tools such as MobaXterm installed. There are ma other options such as:
PuTTY
GitBash which is available by default when you install Git on Windows.
Powershell - This is available by default on every Windows computer. Even though you can use it to access Linux computers remotely, it is more optimised for Microsoft Windows.
for simplicity, you should focus only on MobaXterm which is perfect for all you need throughout this program.
For MacOs users, client terminal is already available so you don't have to do anything. Simply open up the terminal by navigating to the Applications folder --> Open up the Utilities folder -
 And locate "Terminal"


> # CONNECTING USING SSH

Now that you have the terminal open, it is time to connect to the remote server you createc earlier.
Most client tools already have SSH installed, so you literally don't have to do anything other simply typing the command "ssh" on the terminal.
1.    Open up the terminal
2.    Locate the "pem key" you downloaded 
when you provisioned the cloud server.
![](./Images/Connecting%201.png)


3.    Assuming it got downloaded in the "Downloads" folder
![](./Images/connecting%202.png)

4.    Use Linux command to navigate into that folder
* Then we go back to our instance and we active our ec2 on our main computer , more or less like cloning, we put in our ssh private code and it will not be configured "key" file is cont protected as shown below
![](./Images/ssh%20clone.png)

* We head back to our AWS profile to secure the prem file and we will run the code accordiling and we would be able to access our online computer 
![](./Images/ssh%20clone%20cofrimed.png)

* As seen above we now have access to our computer and we are ready to work



Installing, Updating and Removing Software
Since we are already on an Ubuntu based server, lets explore how to install tools on a linux server.



> # INSTALLING, UPDATING AND REMOVING SOFTWARE
1. Updating Package Lists Before installing new software or updating existing packages, it's important to refresh the package lists.
![](./Images/SUDO%20APT.png)

![](./Images/SUDOO%20APT.png)


2. Installing Software Packages
Lets try to install a command called ' tree
The tree command is commonly used to visually see the file system structure on a Linux server 
So let's install it with the command below.
Debian/Ubuntu
![](./Images/SUDO%20TREE.png)


3. Verifying Installed Packages To confirm that the desired package or software has beer successfully installed, simply run the tree command, and specify the path you want t see the tree structure.
 Where the command will bring nothing in the directory cause its empty
 ![](./Images/tree%20directories.png)

 4.  Updating Installed Packages Keep your system up-to-date by updating installed packages.

![](./Images/sudo%20upgrade.png)

5. Removing software packages 
* To remove the "tree" package we installed earlier, we run the following command "sudo apt remove tree"

![](./Images/sudo%20remove%20tree.png)
