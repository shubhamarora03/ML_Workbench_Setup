# Machine Learning Framework for Ubuntu 20.04

1.	If you are a windows user then you must install Oracle Virtual toolbox for installing Ubuntu OS.
- Link for downloading Virtual Box: - [VirtualBox](https://www.virtualbox.org/ "VirtualBox")

2.	Then you must download Ubuntu ISO file 20.04 from the below link.
- Link for downloading Ubuntu ISO file: -[UbuntuISO](https://ubuntu.com/download/desktop#download "UbuntuISO")

![](/Images/UBUNTU.png)

3.	Before installing UBUNTU enable virtualization from BIOS.

4.	Refer the below YouTube tutorial for UBUNTU installation. 
- Link for UBUNTU Tutorial:- [Ubuntu Installation](https://www.youtube.com/watch?v=x5MhydijWmc&t=5s "Ubuntu Installation")

5.	Next Step is to maximize to UBUNTU on Virtual Box.
- Link to maximize UBUNTU:- [Maximize Window](https://www.youtube.com/watch?v=x5MhydijWmc&t=5s "Maximize Window")

6.	Configuring zsh
Open UBUNTU terminal and execute the below commands: - 
sudo apt-get update
sudo apt-get install zsh curl git
zsh (go to zsh)
Press 0

Now configure oh my zsh framework on top of zsh.
- Link for oh my zsh: - [zsh](https://github.com/ohmyzsh/ohmyzsh "zsh")

Copy and paste the below command
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
 
![](/Images/ZSH.png)

Now go to the below directory and change the theme to agnoster
nano ~/. zshrc
ZSH_THEME = “agnoster”
Go back to bash and then zsh (look and feel has changed)

Now you must assign that by default it will select zsh as default
sudo chsh -s $(which zsh) 

7.	Setting up Python Environment using miniconda
Link for miniconda :- https://docs.conda.io/en/latest/miniconda.html
In the terminal, change the directory where the downloaded miniconda is located 
sh Miniconda3-latest-Linux-x86_64.sh
The installation has not modified .zshrc file 
cd /home/shubham/.bashrc (will open this file and copy the below initialize statement)
Copy and paste that snippet in .zshrc file and change the name of shell from bash to zsh.

8.	To set up code server on UBUNTU first open the below link in browser
Open the GitHub link:- [Code Server](https://github.com/cdr/code-server/releases)

![](/Images/CODESERVER.png)

Open the UBUNTU terminal and paste the below commands one by one: -
wget https://github.com/cdr/code-server/releases/download/v3.5.0/code-server-3.5.0-linux-x86_64.tar.gz
ls
tar -xzvf code-server-3.5.0-linux-x86_64.tar.gz
ls
cd code-server-3.5.0-linux-x86_64
. /code-server
PASSWORD = Shubham - - host 0.0.0.0 - - port 20000
