![Hackathon Logo](docs/images/hackathon.png?raw=true "Hackathon Logo")
# Sitecore Hackathon 2024

## Team name
⟹ Sitecore Wizards

## Category
⟹ Best Module for XM/XP or XM Cloud

## Description
⟹ In the thrilling arena of the Sitecore Hackathon, our team, the Sitecore Wizards, have worked on a groundbreaking Media Migration Tool designed to seamlessly transfer media content from Sitecore XP to Content Hub DAM. The Purpose of the module is to facilitate an effortless migration of media assets from XP to Content Hub DAM, by providing necessary credentials to the environment. 

⟹ Currently, there is no direct module available to Migrate the Media from Sitecore to Content Hub. You have to download the media, and upload those media items into Content Hub Manually. Or you can bulk upload manually by creating an import File. 

⟹ This Module, solves the problem of downloading the media items to some location and then reuploading them to Content Hub. Instead, once connected, we can directly upload the media item from Sitecore Media Library to Sitecore Content Hub DAM.

⟹ The Module works for Sitecore XM/XP as well as for Sitecore XM Cloud.

## Video link

⟹ Link to the Video: https://www.youtube.com/watch?v=KgyZI17U_bw


## Pre-requisites and Dependencies

⟹ Our module is requiring specific Sitecore modules or frameworks to function:

- Sitecore XP – Version 10.3.1
- Content Hub (for the purpose of testing this module out, we are going to share credentials to our Sitecore Sandbox account with the Judges)
- Sitecore PowerShell Extensions-6.4-IAR.zip
- Sitecore Management Services 5.2.113.zip


## Installation instructions
⟹ Write a short clear step-wise instruction on how to install your module.  

1. Use the Sitecore Installation wizard to install the [package](Sitecore Media Migration Module-1.0.zip)
2. Once the package is installed, keep the Restart with Sitecore client checked and close the wizard.
<img width="275" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/da2bebaf-e217-47fd-ade1-d7c7df861a55">


## Usage instructions

1.  Next, Open Content Editor, and go to the item: '/sitecore/system/Modules/PowerShell/Script Library/Sitecore Content Hub/Media Migration to Content Hub' and confirm that the checkbox to Enable the Module is checked. In case it is not, please check it manually.
![image](https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/15012fe7-a640-448f-a83f-a3aa85fbf2d3)

2.  Go to Media Library and right click on an Image or Jpeg type of item.
3. The Option to Upload to Content Hub will be available
![image](https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/3550301d-4a31-4a2b-b1b9-56b70a2177f7)

4. A Prompt will appear to ask for Username
![image](https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/5a43cdab-42af-47ff-b1e7-978d8b081a46)

5. Next, a newer Prompt will ask for the Password
![image](https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/6a298cb6-c43d-48b0-8aae-8030abf25d0c)
<img width="201" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/accdc220-c8c3-4321-a854-0437dde417b7">

6. Upon successful authentication, the Module will create a token item in System/Settings, which will be utilized for future uploads to Content Hub
<img width="456" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/f5e0c293-79d1-485d-95b6-3055c9bdffb4">

7. Once the Script Completes, a complete log is available showing the actions performed.
<img width="402" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/554d02b7-a8bb-437c-8329-be19c8a8a6f0">

8. In case the Media Item is already uploaded in the past, the module will skip uploading the item again.
<img width="402" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/08926cf7-8a37-4b55-884c-513e2639b42e">

9. We have created members in M.Asset Definition items, to map Sitecore fields like Item ID, Item Path, Title etc.
<img width="944" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/49982d19-ff73-494b-b5a3-2ef99f4ea266">

10. Also, the Module generates a Public link which can be utilized in Sitecore for future purposes.
<img width="479" alt="image" src="https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/98a51f6e-b79f-4182-a5b2-240a62eec740">



## Comments

Future Enhancements:
- The module can be extended to support Media items other than Image and Jpeg types.
- The module can be extended to have bulk Media Upload, specifically, the whole folder, to have all the media items in Content Hub in one go.
- WE are already generating the public link for the uploaded media items. We could install and configure the Cotnent Hub DAM Connector in Sitecore, and utilize this public link, such that, as soon as the Media item is uploaded in Content Hub, and Public Link is generated, the Module scans the complete content tree, and finds where all the given Media Item ID is available. It can then replace that with the Public Link URL.
