# Hosting Your Resume on Github Pages  
This step-by-step guide will bring you through the process of hosting your own resume on a statically generated website through GitHub Pages.

![My resume in gif form](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/resume.gif)

## Purpose: Guide a User Step-By-Step Through Hosting Their Resume on Github Pages
## Pre-requisites:  
1. A github account
    - If you're new to GitHub, step on over to [github.com](https://github.com/) and create a new account.
    - Don't opt in for the premium plan, a free account is all we need.
2. Ghostwriter markdown editor
    - Ghostwriter is free and can be downloaded [here](https://ghostwriter.kde.org/).
    - Its also handy whenever you want to make changes to your markdown resume as it has a live split preview so you can see any formatting changes immediately.
3. A markdown-formatted resume
	- If you are unfamiliar with writing with markdown, there are some quick starts and guides listed in the [more resources](more-resources) section.

## Getting the Website Template

A practice that Andrew Etter strongly suggests is to host writing on a website instead of creating individual files for distribution. The benefits for this can be clearly seen:
- A single url can be shared repeatedly, this is more lightweight than sending documents over email.
    + Not to mention that any updates/revisions to our written works will be reflected without needing to send a new document.
- Websites are incredibly diverse in structure and format; writing a website perfectly curated for your written work will take it to the next level.

### Forking the Resume Template
1. Navigate to the resume template hosted here
2. Click on the "Fork" button.
3. Set the **Repository Name** to your GitHub username followed by ```.github.io```.
    - For example, my repository would be named ```awphung.github.io```.
    
![The correct fork setup](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/Create%20a%20new%20fork.jpg)
>Warning! If you don't have the "username" part of the repository name set as _exactly_ your username, GitHub Pages won't work.  
4. Click on the **Create fork** button.
5. Wait for the fork to complete.
6. Once complete, navigate to the **Settings** button near the top of the repository.
7. Then, look down the sidebar until you see the **Pages** button under the **Code and automation** section.
8. Change **Branch** to **gh-pages**.
9. Click save.

You have successfully forked a resume template to your GitHub account, and now you're ready to start making this template your own! 

Our next step is getting the repository on your local machine so you can start pushing changes.

## Preparing the Template Repository for Modification
### Installing GitHub Desktop
1. Navigate to the GitHub Desktop [download portal](https://desktop.github.com/)
2. Click on the download button for your operating system.
3. Wait for the installer to complete the installation.
4. Once completed you should see this:  
![GitHub Desktop Home](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/Github%20Desktop%20start.jpg)

### Getting Your Repository on Your Local Machine
1. Click on the "Clone a repository from the Internet..." button.
2. Sign in to your GitHub account.
3. Under "Your repositories" select your forked repository from earlier.
4. Select your desired local path for the repository.
>Note: When picking a local destination for your repository, pick a directory that is empty to avoid any conflicts while cloning.
5. When prompted, select the "For my own purposes" option.
6. Click on the continue button.
7. Now your GitHub Desktop should look like this:  
![GitHub Desktop in repo](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/Github%20Desktop%20Cloned%20Repo.jpg)

## Modifying the Resume Template

Thanks to magic of Distributed Version Control Systems (DVCS), modifying your resume website template is as easy as making the desired local changes and pushing them to this repository.  

Etter believes that we should treat our written works as a working draft; meaning changes should be regular and expected. This approach to changes makes sense especially for resumes, which are constantly being updated as we grow and change as professionals. Whether its a small adjustment to a work experience or a complete format overhaul, hosting our resume on a DVCS ensures it is always up to date.  

Now onto the fun part; getting your resume into this template and making it yours!

### Changing the Configuration File
1. Open ghostwriter.
2. Click on the **File** button on the top.
3. Hit the **Open** button next.
4. Navigate to the directory you cloned your repository into previously.
5. Open ```_config.yml```.
6. Now, change the following as instructed:
7. On line 1, replace ```Researcher``` with your full name.
8. On line 2, replace ```https://ankitsultana.com``` with your repository name.
    - For example, I'd put ```awphung.github.io``` here.
>Warning! **Do not** remove the quotation marks around the **url:** text there when you modify this line.
9. On line 3, delete all the text so you only have ```"\"``` remaining
10. Delete lines 18-24.
    - These are navigation buttons for a sidebar, which we most likely won't for a standard resume. 
11. Save the config file.

## Modifying the Resume

This next step deals with the ```index.md``` file in the repository. This is where your markdown-formatted resume's content will be stored.  

Etter heavily supports the use of lightweight markup languages for many reasons, one of which is the simplicity of writing in these languages. There is no need for proprietary formatting conversions or complex syntax to get acquainted with (**ahem**, LaTeX).

### Changing the Index File
1. Open your markdown-formatted resume in ghostwriter.
2. Copy all of the content in your resume.
3. Now open ```index.md``` in ghostwriter.
4. Note the first 4 lines of code, do **not** modify them.
>If you do the layout will be ignored or incorrect.
5. Replace the rest of the content in this file with your copied resume content.
6. Save this file.

With these modifications, your resume is now set up be formatted by GitHub Pages' static site generator! Now all we have to do is get these new changed files onto your repository.

## Pushing the Changes
1. Open up GitHub Desktop.
    - You will see something that looks like this:
![GitHub Desktop changes shown](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/Github%20Desktop%20Changes.jpg)  
2. Navigate to the **Summary (required)** text field near the bottom left corner.
3. Summarize the changes made.
    - You can also add a more detailed description if you wish, but that is optional.
4. Click the **Commit to gh-pages** button on the bottom left of GitHub Desktop.
5. Now, hit the **Push origin** button on the top toolbar or in the blue highlighted section.
![Push to origin buttons](https://github.com/awphung/awphung.github.io/blob/gh-pages/resources/Github%20Desktop%20Push.jpg)

:tada:Congratulations, you've just pushed your resume onto your repository! That means your resume is ready to be processed and statically generated into a website! Keep in mind it will take a couple of minutes to generate it, so take this time to continue reading this readme for some cool tips :sunglasses:.

## <a name="more-resources"></a>More Resources
- This [Markdown tutorial](https://www.markdowntutorial.com/) is a great place to get started with Markdown. It provides little lessons so you can get hands on when learning.
- In case you haven't already read Andrew Etter's book _Modern Technical Writing_ cover to cover already, you can check it out [here](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS). It covers a plethora of useful topics to help you convey technical information in a concise manner and more.

## Acknowledgements
- Group 6 Members Aaditya Raj Gupta, Luxiang Lin, and Mahamud Hasan Asif for their wonderful peer feedback on this readme and my resume.
- ankitsultana for their [Jekyll resume template](https://github.com/ankitsultana/researcher).

## FAQs

### Why is Markdown better than a word processor?
A big draw to Markdown is the lack of compatibility issues that plague other word processors such as Microsoft's Word. Because we are tied to a specific format or list of formats when using a word processor, things like cross platform collaboration can be very time consuming and frustration-riddled. Ever convert a LaTeX file to PDF and then open that PDF in Word? It sucks. Markdown on the other hand is near universal, can be edited at full capacity with any text editor, and file sizes tend to be much smaller in comparison to other popular document formats.  

### What else can I do with my resume website? 
Pretty much anything you can dream of! If you just want to update your resume's content, simply update ```index.md``` and push the changes to this repository. If you want to get a bit serious with it, there's tons of Jekyll based resume formats available online that you can apply to this repository. Not to mention the plethora of things you can accomplish with a bit of Javascript and CSS; its just like any other statically generated website! 
