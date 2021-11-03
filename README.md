# Hosting a Resume to a static website
---
**Purpose:** A step-by-step instruction of how to host a résumé to a static website using Markdown, GitHub pages and Jekyll by applying the principles of current technical writing according to the book *Modern Technical Writing* by Andrew Etter. 

---
**Prerequisites:**  
* Must require a Markdown formatted resume  
* Know what is a distribution version control system like GitHub, GitLab etc  
* Be able to install Git in your operating system 
---
**Instructions**  
## 1) Write a resume using a Lightweight Markup Language  
>Etter states that the use of Lightweight Markup Language is important because it is easy to make well-formed XML by utilizing it, which is essential to create websites. He proposes the use of Markdown because of its simple syntax, although it has some limitations which influences the creation of different flavors. Markdown is also considered to be the most popular Lightweight Markup Language in the world and because of its popularity there are many specialized editors, such as:  
>* [MarkdownPad](http://markdownpad.com/) (Windows)
>* [iA Writer](https://ia.net/writer) (Mac OS)
>* [ReText](https://www.linuxhelp.com/how-to-install-retext-7-0-1-on-ubuntu-18-04) (Linux)  

### Markdown resume  
i) Confirm that your resume follows [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/)  
**Note**: Using GitHub Flavored Markdown is essential while hosting markdown files to GitHub Pages




## 2) Create a GitHub Account and Create a repository
>Etter emphesizes on the use of distribution version control systems (DVCS) because DVCS provide better performance, facilitate working offline and are efficient while working on concurrent files. Also, modern software developers favor the use of such technology and would prefer to have their code and documentation stored at the same place.  
  
[Github](https://github.com/) is an excellent choice for a DVCS as it is the worlds largest open source repository with benefits such as:
* Cloud storage for source code
* Supports all popular programming languages 
* Streamlines iteration process

Since we will be using **GitHub Pages** to host our resume having a GitHub account is **necessary**.

### Install Git
i) Clink the [link](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and follow the instructions for your operating system.

### Joining GitHub  
i) Click the [link](https://github.com/login)   
ii) Click on "Create an account"  
iii) Go through the step-by-step process prompted on the screen  

### Creating a New Repository
i) Login to [GitHub](www.github.com)   
ii) Click on Repositories    
iii) Click "New" which is the green button on the top right  
iv) Select the TextBox labelled "Respository Name" and write "\<YOUR USER NAME\>.github.io"  
**Note**: The naming format must be followed as given, simply change the first part to your user name (do not include the <>)  
v) Click "Create Repository"  

### Push your Resume to the online Repository    
i) Go to your repository and click "code", you should see a URL  
ii) Click on the URL and copy it  
iii) Open the command line tool and locate to the directory where you wish to download your repository and write the follow command  
```
	git clone <URL>
```  
This command will download your repository to your local machine  
iv) Rename your resume to "index.md" and paste it to the local repository  
v) Type the following in the command line tool (make sure you are located in the directory of your local repository) 
```
	git add *
```  
```
	git commit -m<commit message(optional)>
```  
```
	git push
```  
This will successfully upload your resume into your online repository  



## 3) Hosting on GitHub Pages  
>Static Websites are great for documentation, some benefits mentioned by Etter are, they having no dependencies and easy migration.
GitHub pages uses Jekyll to host static sites and even allows the option of adding styles to documentation known as themes, which gives your documentation a more professional and consistent outlook.

The steps needed to host a static website with a theme are:  
i) Go to your online repository and click on "settings"  
ii) Scroll down to find the "GitHub Pages" section and click on the link to redirect to the GitHub pages panel  
iii) Make sure the source is selected to "main"  
iv) Click "Choose Theme" which should redirect to a page that displays the different types of themes available  
v) Choose your desired theme and click "Select Theme"  
vi) Scroll down and press "Commit Changes"  
vii) Open a web browser and type in "\<YOUR USER NAME\>.github.io", to view your resume on a static website  


The website should look something like this:  
![AnimatedGif](https://media.giphy.com/media/eLSfc5a1vWQ9KyJDQu/giphy.gif)


### More Resources
* [MarkDown Tutorial](https://www.markdowntutorial.com/)  
* [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) by Andrew Etter  
* [GitHub Pages](https://pages.github.com/) has more information about utilizing its fucntionality 

---

### Authors and Acknowledgments:   
This document was written by Farhan Akib Rahman, using Andrew Etter's book *Modern Technical Writing* as reference. Reviewed by Haseeb Paracha, Akshay Sharma, Zhijie Zheng and Kien Mai

---
### FAQs

1) **Why is my resume not displaying the theme I selected?**  
>If the markdown file is not written in Git Hub Flavored format the system will not render it accurately, which will cause the website to look different and the theme to not show up.

2) **Do I have to use GitHub to host my static webpage?**  
>No, a static site can be manually hosted by using a generator like Jekyll or Sphinx, by providing a lightweight markup and a theme. The site can be updated by editting the content and processing everything again.  

3) **Why are the changes I made to my resume not displaying in my static website?**  
>Go to your index.md file through your site (<username>. github.io/index.md) and then reload the page. Then you can go back to (<username>.github.io) and it should have updated.

4) **Why is Markdown better than a word processor?**  
>Although word processors are great for creating pdfs, it is not useful for websites because you need to style it as you are writing. Whereas, markdown takes advantage of html and css to set consistent styles.










