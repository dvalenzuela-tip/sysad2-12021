## 1. How to create an Ansible Configuration  

#### First step:  
  Make sure that the ansible.cfg or Ansible configuration is already installed in your system by executing the command `ansible --version`  

#### Second step:  
  If it is already installed, enter the command `apk add ansible`. If it is already installed you may now create the ansible configuration file by using the command `touch ansible.cfg`   

#### Third step:
  After creating a file, you may now create a configuration inside of the ansible configuration file using a text editor using the command `vim ansible.cfg` 


## 2. How to create an Ansible Inventory  

#### First step:
  In the same directory where the ansible configuration or ansible.cfg file is created, you must create a file which will serve as a inventory file. You can create it with the command `touch inventory`
#### Second step:
  With the use of text editor such as vim or vi, you can input the command `vim inventory` and inside of that you must input the ip address for example [ubuntu] and under of that text will be the ip address of your server in order to access it.  

#### Third step:
  After you do the first and second steps, you must save it by pressing the ESC button and type the command `:wq!` to write and save it.

#### Fourth step:
  You may check your inventory file to be make sure that the file is created successfully with a correct configuration just like for example you put an IP address of your ubuntu server on it and you want to test it by pinging it. By that you can use the command `ansible all -m ping`


## 3. How to create an Ad-hoc Ansible command with setup and shell module.  

#### First step:
  First, you need to setup the hostname by executing the command `(your hostname) -m setup (file name)`

#### Second step:  
  Next, you must display the output of the file that you setup in the previous set of commands by executing the command `ansible (your hostname) -m shell -a`







