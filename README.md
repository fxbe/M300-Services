# M300 Documentation

<br>

# K1

<br>

### Preparation <br>
- Install Virtualbox
- Install Vagrant
- Install VS Code
- Install Git Client
- Generate SSH-Key on Client
- Add SSH-Key to Git
<br>

# K2 <br>

Git Account: <br>
- Login Mail: 	fabkel2002@gmail.com <br>
- Passwort: 	******* <br>
<br>
Current knowledge: <br>

- Linux: <br>
	I've been working with Linux for the past few months so I know the basics like how to navigate through a machine or how to edit files with "Vi".  <br>
	
- Virtualization <br>
	Virtualization is a big part in IT and is also used a lot in our company. We are using Swisscom Private Cloud. <br>
	I have also had a couple of school-modules were this was needed. <br>
	
- Vagrant <br>
	I have never used Vagrant prior to this modul. <br>
	
- Git <br>
	I'm working with Git everyday in my workspace. <br>
	
- Mark Down <br> 
	Mark Down is a big part of Git because it is the documentation of your project in Git or is an installation process to get your Git project working so I'm also using it everyday. <br>
	
- Systemsecurity <br>
	There was alot of new things in this part but I knew a couple before. <br>
<br>
My new knowledge <br> 
	
- Vagrant <br>
	VAgrant is a tool to make the provisioning of VM's easier and do it all with one command. This can be especially usefull in cases where you need more than just one VM on different servers provisioned. <br>
	Basic Vagrant commands: <br>
- Vagrant init: creates the Vagrant file <br>
- Vagrant up: creates the VM according to your Vagrant file <br>
- Vagrant ssh: SSH connection to the VM <br>
- Vagrant status: status of the VM <br>
- Vagrant port: shows the forwarded ports <br>
- Vagrant halt: stops all running VM's <br>
- Vagrant destroy: delets the VM's <br>

- Mark Down <br> 
 	Mark Down is a language used by GIT to display installation steps or in our case <br>
	the documentation of this modul (M300).
<br>

# K3 <br>

### Vagrant <br>
<br>
<br>
These are the things that I changed in the Vagrant file: <br>

- config.vm.hostname = "srv-nv" (Hostename) <br>
- config.vm.network "public_network", ip: "192.168.55.69" (Network) <br>
- vb.memory = "2048" (VM memory) <br>
- vb.cpus = "2" (CPU cores) <br>
<br>
With this comment : <br>

ifconfig: inet addr:192.168.55.69 <br>
hostname: srv-nv <br>
The resource settings can be viewed in Virtual Box. <br>

# K4 <br>
- Install Apache Webserver: <br>

    sudo apt-get update <br>
    sudo apt-get upgrade <br>
    sudo apt-get install -y apache2 <br>

- Firewall configuration: <br>

	sudo apt-get install ufw <br>
    sudo ufw default deny incoming <br>
    sudo ufw default allow outgoing <br>
    sudo ufw allow 80/tcp <br>
    sudo ufw allow 443/tcp <br>
    sudo ufw allow 22/tcp <br>
    echo "y" | sudo ufw enable <br>

- User with admin priviledges: <br>

    sudo adduser localadmin <br>
    sudo adduser localadmin sudo <br>
# K5 <br>

### Reflexion zum Modul 300 <br>
Der Anfang fiel mir einfach, da ich einiges davon bereits im Betrieb hatte und auch schon viel darüber selbst erkundet habe. Die Schwierigkeiten kamen dann als ich mit Vagrant angefangen habe da dies eigentlich das einzig Neue für mich war. Ich habe dort aber einiges dazu lernen können. <br>
