<img src="https://i.imgur.com/C11N4nJ.png" alt="Azure" width="400">

<h1> Creating VM's in Azure: Windows 10 and Linux (Ubuntu) </h1>

<h2> What is a Virtual Machine (VM)? </h2>
A Virtual Machine (VM) is a software-based emulation of a physical computer that runs an operating system and applications like a real computer. It is hosted on a physical machine, which can support multiple VMs simultaneously. Each VM operates independently, with its own virtual hardware components such as CPU, memory, storage, and network interfaces. VMs are commonly used in cloud computing, software development, testing, and server consolidation because they allow for flexible, efficient, and isolated computing environments.
<h2> Overview </h2>
In this tutorial, we'll create two Virtual Machines (VMs) in Microsoft Azure: Windows 10 and Linux. 
In [Part 2](https://github.com/Kelsow96/Network-Security-Groups-NSGs-and-Observing-Network-Traffic) of this project, we'll work with Network Security Groups (NSGs) and use WireShark to observe network traffic between our two VMs.

<h2> Environments and Technologies Used: </h2>

- Microsoft Azure (Virtual Machines/Compute)

<h2> Operating Systems Used: </h2>

-  Windows 10
-  Linux (Ubuntu)

<h2> List of Prerequisites: </h2>

-  Azure Account/Subscription

<h2> High-Level Steps: </h2>

 1. Creating a Resource Group within Azure to hold our VMs in
 2. Creating our Windows 10 VM with the correct configurations within our made Resource Group
 3. Creating our Linux(Ubuntu) VM with the correct configurations within our made Resource Group

<h2> Steps: </h2>

- First we'll create a resource group within Azure to hold our VM's in. We'll call it WireShark_Lab.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/1756fd76-67ee-4e25-8831-9704f2ae48a7)
  <br />
  <br />
  
- Next we'll create our first VM: Windows 10
  <br />
  <br />
  
- It will be held in the resource group we just made (WireShark_Lab), we'll call it Windows10-VM and we'll select the Windows 10 Image.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/727270e5-5659-418b-a2e9-a4ea8eedc444)
  <br />
  <br />
  
- We'll change the computing power size, create a Username and Password and confirm the licensing agreement at the bottom.
  - We'll use Jane as the Username and Password1234 as the Password to keep it simple.
  - Username: Jane , Password: Password1234
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/ec591353-34f6-4cdc-84e8-22e53544799f)
  <br />
  <br />

- We'll move onto Review + create and if we did everything correctly it should pass validation and we'll be able to create the VM.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/f5f31191-533c-401f-aa8b-24373f60b7f6)
  <br />
  <br />

- Next we'll create our second VM: Linux (Ubuntu)
  - We'll use the same steps as before when creating our first VM but changing a few things.
  <br />
  <br />

- It will be held in the resource group we just made (WireShark_Lab), we'll call it Linux-VM and we'll select the Ubuntu Server Image
 ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/e000d19b-6794-4e32-aa66-4081e4e56669)
  <br />
  <br />

- We'll change the computing power size, change the Authentication type from the auto-selected SSH public key setting to Password and then we'll create a Username and Password. Once thats done we'll go back to top and select Networking.
  - We'll use Jane as the Username and Password1234 as the Password as before to keep it simple. 
  - Username: Jane , Password: Password1234
![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/a1d10cc0-3371-418c-b21c-e64281bb1376)
  <br />
  <br />

- Go back to the top and select Networking.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/23305f1d-97e2-4ecf-b89a-64c1c96e5661)
  <br />
  <br />

- Once in Networking we'll confirm that our Virtual network is within Windows10-VM-Net and that our Subnet is within the defualt.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/0054e4c9-62e6-4726-9640-60224026df17)
  <br />
  <br />
  
- We'll move onto Review + create and if we did everything correctly it should pass validation and we'll be able to create the VM.
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/36825d8a-8fab-48d8-9056-63db2f5eb666)
  <br />
  <br />

- We should now see both of our VM's and the resources they created within our WireShark_Lab Resource group
  ![Capture](https://github.com/Kelsow96/Creating-VM-s-in-Azure-Windows-10-and-Linux-/assets/169297569/ffd63280-8f91-494b-9885-11dde5b53af3)
  <br />
  <br />

- Now that we have our VM's created we can move onto [Part 2](https://github.com/Kelsow96/Network-Security-Groups-NSGs-and-Observing-Network-Traffic) of this project where we'll be working with Network Security Groups (NSGs) and using WireShark to observe network traffic between our two VMs.



  







