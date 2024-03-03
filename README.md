![Hackathon Logo](docs/images/hackathon.png?raw=true "Hackathon Logo")
# Sitecore Hackathon 2024

- MUST READ: **[Submission requirements](SUBMISSION_REQUIREMENTS.md)**
- [Entry form template](ENTRYFORM.md)
  
# Hackathon Submission Entry form

> __Important__  
> 
> Copy and paste the content of this file into README.md or face automatic __disqualification__  
> All headlines and subheadlines shall be retained if not noted otherwise.  
> Fill in text in each section as instructed and then delete the existing text, including this blockquote.

You can find a very good reference to Github flavoured markdown reference in [this cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). If you want something a bit more WYSIWYG for editing then could use [StackEdit](https://stackedit.io/app) which provides a more user friendly interface for generating the Markdown code. Those of you who are [VS Code fans](https://code.visualstudio.com/docs/languages/markdown#_markdown-preview) can edit/preview directly in that interface too.

## Team name
⟹ Sitecore Wizards

## Category
⟹ Best Module for XM/XP or XM Cloud

## Description
⟹ In the thrilling arena of the Sitecore Hackathon, our team, the Sitecore Wizards, have worked on a groundbreaking Media Migration Tool designed to seamlessly transfer media content from Sitecore XP to Content Hub DAM. The Purpose of the module is to facilitate an effortless migration of media assets from XP to Content Hub DAM, by providing necessary credentials to the environment. 

⟹ Currently, there is no direct module available to Migrate the Media from Sitecore to Content Hub. You have to download the media, and upload those media items into Content Hub Manually. Or you can bulk upload manually by creating an import File. 

⟹ This Module, solves the problem of downloading the media items to some location and then reuploading them to Content Hub. Instead, once connected, we can directly upload the media item from Sitecore Media Library to Sitecore Content Hub DAM.

## Video link
⟹ Provide a video highlighing your Hackathon module submission and provide a link to the video. You can use any video hosting, file share or even upload the video to this repository. _Just remember to update the link below_

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

3.  Next, Open Content Editor, and go to the item: '/sitecore/system/Modules/PowerShell/Script Library/Sitecore Content Hub/Media Migration to Content Hub' and confirm that the checkbox to Enable the Module is checked. In case it is not, please check it manually.
![image](https://github.com/Sitecore-Hackathon/2024-Sitecore-Wizards/assets/80135943/15012fe7-a640-448f-a83f-a3aa85fbf2d3)

4.  Go to Media Library and right click on an Image or Jpeg type of item.
5. The Option to Upload to Content Hub will be available
6. profit

## Usage instructions
⟹ Provide documentation about your module, how do the users use your module, where are things located, what do the icons mean, are there any secret shortcuts etc.

Include screenshots where necessary. You can add images to the `./images` folder and then link to them from your documentation:

![Hackathon Logo](docs/images/hackathon.png?raw=true "Hackathon Logo")

You can embed images of different formats too:

![Deal With It](docs/images/deal-with-it.gif?raw=true "Deal With It")

And you can embed external images too:

![Random](https://thiscatdoesnotexist.com/)

## Comments
If you'd like to make additional comments that is important for your module entry.
