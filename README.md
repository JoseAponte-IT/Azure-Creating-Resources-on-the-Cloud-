![screenshot azure](https://github.com/user-attachments/assets/2f08cc48-fe99-4267-bbc8-a886cc77c332)
# Azure: Creating Resources on the Cloud
<p>This project demonstrates how to leverage Microsoft Azure to create and manage cloud resources, showcasing both technical proficiency and an understanding of fundamental cloud concepts. Follow along as we create a Resource Group and deploy Virtual Machines within it, accompanied by detailed explanations and screenshots. 🫡
</p> 

<h2>Technologies used </h2>

- Microsoft Azure: Cloud platform for managing resources and applications <br>

-  Azure Virtual Machines (Windows and Linux [Ubuntu])

- Azure Portal: Web-based interface for cloud resource management
    
- RDP: A protocol used for remotely accessing and controlling virtual machines
  
<h2>Key Concepts</h2>

- Cloud Computing: When resources or computing services are given over the internet, allowing on-demand access and scalability

- Azure: Microsoft's cloud platform for building and managing cloud solutions

- Resource: A service like a database, VMs or storage that can be created , managed , and used in Azure

- Virtual Machine (VM): A computer within a computer, it's software that uses resources allocated to it (CPU,RAM,etc) to emulate a computer with its own operating system and applications

<h2>Prerequisites</h2>

- An active Microsoft Azure Subscription will be needed to do this lab 

# Project Overview
<h2>Step 1: Create a Resource Group</h2>

<p>This will serve as a container of sorts (like a folder) that will hold our resources (Virtual Machines)</p>

- Go to Azure Portal

![image](https://github.com/user-attachments/assets/6f75e551-4d66-4af6-a20e-8a1f6fa831fe)

- Go to Resource Group

![image](https://github.com/user-attachments/assets/37506426-1785-44af-8dff-d2fbf4735d20)

- Create Resource Group

![image](https://github.com/user-attachments/assets/d1571f43-284a-4721-b0ad-1d170b33273e)

- Name the Resource Group

![image](https://github.com/user-attachments/assets/c45b31c1-83c8-4e6e-8e25-20b0be0eb104)

- Review and Create Resource Group

![image](https://github.com/user-attachments/assets/b98e48a6-a504-44df-899a-2b91a9354f7e)

- Create Resource Group

![image](https://github.com/user-attachments/assets/cfa87af7-f3c9-44aa-8912-4d34c05ed2b8)

- Resource Group Succesfully created

![image](https://github.com/user-attachments/assets/c2859c23-b3cb-4c60-89ca-c436937415ed)

<H2>Step 2: Creating Resource (Virtual Machine)</H2>

- Return to the Azure Portal and find the "Virtual Machines" option (You can search it in the searchbar if you cant find the option in the dashboard) 

![image](https://github.com/user-attachments/assets/37ac9f7a-e86c-44b7-aa37-d125469a692f)

- Create a virtual machine resource 

![image](https://github.com/user-attachments/assets/64829dcf-3278-4353-a19d-dc6f9425a77f)

- Assign the VM to the Resource Group that was created

![image](https://github.com/user-attachments/assets/d101a9e4-3db9-4de2-b485-556884d23b03)

- Fill out these details:<br> 
-Virtual Machine Name<br>
-Region [!!IMPORTANT!! Make sure that the region used to create the resource group is the same as the region as the VM you are creating, might run into issues otherwise] <br>
-Image [we are going to make a Windows 10 vm so make sure to select the Windows 10 pro option for image]<br>

![image](https://github.com/user-attachments/assets/6d08279c-cba8-4fa2-94d2-1f180a82f7e9)

- For optimal performance I will use 2cpus as the standard size<br>

![image](https://github.com/user-attachments/assets/08cfa758-8454-4343-9665-f5081ebfdd80)

- Create Username and password 

![image](https://github.com/user-attachments/assets/028d853e-63a4-4d23-938e-b3c39daa1d01)

Confirm Licensing 

![image](https://github.com/user-attachments/assets/d25e7c66-a950-461c-a7fb-6e1109460123)

- Review and Create 

![image](https://github.com/user-attachments/assets/bdce6266-ec36-43a7-9aaa-9ec34b2c6a10)

![image](https://github.com/user-attachments/assets/dd270697-8d60-4b08-944e-e45ddae3e3ca)

- Virtual Machine (Windows 10 Pro) Successfully Created.<br>
Osbervations: When creating our VMs, a Virtual Network,Virtual NIC, IP Address abd Network Security Group will be automatically created.<br>[Essentially all the necessary network infrastructure so that the Vm can have its own network to transfer data locally and to the internet]  

 ![image](https://github.com/user-attachments/assets/8b856f5e-c4e7-4184-9aa2-6d57d43d3930)

<h2>Step 3: Creating our Second Resource (Virtual Machine)</h2>

- Repeat same Steps as before to create our second VM(Linux Ubuntu server):<br>
Place vm in the same resource group as the other VM we made<br>Name VM<br>Use the same Region as the resource group<br>Choose 2cpus for the size for optimal performance<br>Select Authentication Type Password<br>Create a Username and password<br>Review and Create

![image](https://github.com/user-attachments/assets/acb2ad8a-26eb-45d1-82ca-1e9596130a93)

![image](https://github.com/user-attachments/assets/7fade3dc-6004-4450-a2e3-2929758ca719)

![image](https://github.com/user-attachments/assets/6ef7e8d4-3c7e-4167-9d00-233eea290693)

![image](https://github.com/user-attachments/assets/b9c01a26-9fa1-4807-8839-c479bc7bed41)

- Virtual Machine (Linux Ubuntu) Successfully Created<br>
🎉 Congrats you have now made 2 Virtual Machine resources using the cloud 🎉

![image](https://github.com/user-attachments/assets/dd040ee5-9e06-40a2-a3f5-0ecc74aa26b2)

![image](https://github.com/user-attachments/assets/21b32eb1-23cf-4f69-a5c3-fa7e389d022c)

<h2>Step 4: Use RDP to check if VM's are running (optional) </h2>

- Return to the Virtual Machine Dashboard in the Azure portal

![image](https://github.com/user-attachments/assets/a2e686dc-d035-432b-a079-18927560bc76)

- Jot down the Public IP adresses of the VM's 

![image](https://github.com/user-attachments/assets/1a8e4a73-f175-42fb-bb68-6ba3ab1b18ba)

- If on Windows press Windows key -> Open RDP If on MAC download RDP program in APP store and put in the IP adress of one of the VM 

![image](https://github.com/user-attachments/assets/5f159faa-a725-4e26-b101-de3f7121278e)

- Enter the Log in credentials and log in to the machine 

![image](https://github.com/user-attachments/assets/bdd8e711-4ed7-4a70-b81a-9a21dd664c23)

- To connect to the Linux VM Remotely open up Powershell or whatever Commandline Interface your OS is using 

![image](https://github.com/user-attachments/assets/7844c01c-08fb-4506-903b-c14106e968f8)
 
-Type in these commands ssh (insert the username of the vm linux machine here)@(insert the IP address of the machine here) press enter

![image](https://github.com/user-attachments/assets/5c1cfc4b-6d81-4c77-92c9-5ffa1314af63)

- Type in the password [it will be invisible as you type it out for security purposes]

![image](https://github.com/user-attachments/assets/b3d3ff20-007f-4a03-bd19-aff14dfcaa6e)

- You have successfully remotely and securely accessed the Linux VM through the means of SSH Yippeee<br>
To exit out of the Linux VM use the command " exit "  

![image](https://github.com/user-attachments/assets/a0052824-fa7b-4cad-84bd-6d31ed8ec863)


🎉Congrats we have successfully remotely logged into the VM's and confirmed that they are running🎉

# That Concludes this lab 🫡




