![image](https://github.com/user-attachments/assets/11629eb8-20a3-46b2-81e7-770f03c61325)

<h1>Implementing a Help Desk Ticketing System (osTicket) in a Windows Local Webserver</h1>

## Languages and Utilities Used

- PHP
- IIS
- 

## Environments Used

- Oracle VirtualBox
- Windows 10 (Pro)
- MySQL

# Setup

## 1. Install Oracle VirtualBox
- **Description**: Download and install Oracle VirtualBox on your machine.
- **Extension Pack**: [Download here](https://www.virtualbox.org/)

---

## 2. Download ISO Files
- **Description**: Download the necessary ISO file for Windows 10 Pro.
  - [Windows 10 Pro](https://www.microsoft.com/en-us/software-download/windows10)

---

## 3. Create Virtual Machines

### Windows 10 Pro VM
- **Description**: Set up a virtual machine for OsTicket.
- **Image**:  
![image](https://github.com/user-attachments/assets/fda4b4c4-5be6-4a32-ab4f-4ee769d3d80d)
![Screenshot from 2024-10-24 13-52-00](https://github.com/user-attachments/assets/45c9161b-1843-4451-ae7f-38485ffb888e)
### Setup:
  - *Allocate 8 GB of RAM and 4 CPUs for better performance.*
  - *Set the hard drive size to 50 GB, which is sufficient for this setup.*
  - *Set up credentials for the Windows account.*
  #### Once the virtual machine is running, we’ll want to enhance the display:
    Go to “Devices” in the top menu and select “Insert Guest Additions CD Image.”
    Follow the prompts to install the guest additions, then reboot your VM.

---

## Enabling IIS

### Now, let’s set up Internet Information Services (IIS), which is Microsoft’s web server:

Open the Control Panel, type “Turn Windows features on or off,” and select it.
![Screenshot from 2024-10-24 14-11-52](https://github.com/user-attachments/assets/acc0c854-6cf5-4a3d-b3be-f8e28da54508)


Check Internet Information Services and make sure the following are selected:
- World Wide Web Services
![Screenshot from 2024-10-24 14-13-44](https://github.com/user-attachments/assets/cbfec0ae-90f4-4de1-b860-47b891be7616)

- Application Development Features (enable CGI)
![Screenshot from 2024-10-24 14-13-52](https://github.com/user-attachments/assets/e2a4f7ed-efce-4b56-a776-6c3a438a933f)

- Management Tools (IIS Management Console)
![Screenshot from 2024-10-24 14-14-04](https://github.com/user-attachments/assets/b595a386-efd2-4094-86cf-9b3671374750)


### Click “OK” to install IIS.
