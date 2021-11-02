# Readme

A description of how to host and prepare a résumé using Markdown, GitHub pages, and Jekyll relating to the principles of current technical writing according to the book *Moder Technical Writing* by Andrew Etter.

### Markdown formatted resume

```
# Farhan Akib Rahman
163 Thatcher Dr, Winnipeg, MB, R3T 2L7  
+12046981935 | akib1010@gmail.com | rahmanf1@myumanitoba.ca  

---
### Education
 
* 4th Year at Faculty of Science, Major in Computer Science ~ 2018-present  
University of Manitoba  
GPA: 3.7/4.5  
Expected Date of Graduation: May 2022  

---
### Related Skills   

**Technical** 
 
| Languages| Java, Python, JavaScript, C/C++, SQL, HTML, System Tap|
------------ | -------------
 **Software**| **Vim, VS code, IntelliJ, R Studio, Android Studio, MS Excel, MS Word, MS Powerpoint**
 **Operating Systems**| **MS Windows, Mac OS, Red Hat Linux**


**Leadership**  

* Supervised and trained personnel in a retail store to ensure that the store's values and mission are upheld among employees and that exceptional customer service is maintained
* Demonstrated management skills by organizing tasks and facilitating communication between team members during a software development project
* Captained a first division basketball team, coached and motivated the team to perform at their maximum potential


---
### Work Experience 
 
 **Customer Experience Salesfloor Associate** ~ 2018-2019  
Walmart, St Vital Center, Winnipeg, MB  

* Providing excellent Customer Service by greeting all customers in a polite and friendly manner, assisting customers by promoting products/services, locating merchandise and making purchase decisions, resolving customer issues and referring concerns where appropriate
*  Covering and zoning an assigned area(s) on the salesfloor
*  Communicating with other associates to ensure floor coverage is maintained

### Volunteer Experience

**Peer Advisor** ~ 2017-2018  
International College of Manitoba

*  Assist in all matters associated with student welfare, including course advice and
academic performance, and ensuring access to appropriate referral and advocacy
services
* Assist with the implementation of programs and services which promote the wellbeing of students throughout their studies. 
* Assist with the implementation and monitoring of programs and services which assist
with the development of study skills

---

### Projects

**Good Habits**

* Designed and developed an android application with a team
* Followed best design principles and practices to optimize user experience
* Achived high level of assesment from supervising instructor after evaluation

**Web Scraper**

* Developed a program to scrape data from selected websites
* Implemented using python library (BeautifulSoup) and HTML

**Non-Interactive Shell**

* Implemented a non-interactive command line interface with pipes and redirection support, using C++

---
### Awards

Dean's Honour List, Faculty of Science ~ 2020-present

---

### Interests

Web design, Software Development, Sports, Music and Cooking

```

# 1) Write a resume using a Lightweight Markup Language
For this step the most preferred language is Markdown, according to Andrew Etter in his book Moder Technical writing 
>“it is the most widely used markup language in the world” 

mainly because of its simplicity. Etter emphasizes on using this type of language because it is more human-readable, has a smaller learning curve and requires less characters. Some syntax’s of using Markdown are:

i) Adding a ‘#’ at the beginning of a sentence followed by a white space to indicate that it is a heading. For example "\# Farhan Akib Rahman" would produce
	
 # Farhan Akib Rahman 
 **Note**: Adding an extra '#' would give a smaller heading, there can be six sizes for headings the smallest corresponding to '######'. 
 
ii) Wrapping a text with ** would make it bold. For example  "\*\*Good Habits\*\*" would produce 

**Good Habits**

iii) Wrapping a text with * would make it italics. For example "\*Modern Technical Writing\* would produce

*Modern Technical Writing*

**Note**:Using a [GitHub flavored Markdown](https://github.github.com/gfm/) format is necessary for rendering a md formatted file in GitHub Pages. 

Some popular editors for Markdown suggested by Etter are:  
* [MarkdownPad](http://markdownpad.com/) (Windows)
* [iA Writer](https://ia.net/writer) (Mac OS)
* [ReText](https://www.linuxhelp.com/how-to-install-retext-7-0-1-on-ubuntu-18-04) (Linux)

# 2) Create a GitHub Account and Create a repository
Etter emphesizes on the use of distribution version control systems (DVCS) because modern software developers favor the use of such technology and would prefer to have their code and documentation stored at the same place.  
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



# 3) Hosting on GitHub Pages  
Static Websites are great for documentation, some benefits mentioned by Etter are, having no dependencies and easy migration.
GitHub pages uses Jekyll to host static sites and even allows the option of adding styles to documentation.
The steps needed to host a static website with a theme are:  
i) Go to your online repository and click on "settings"  
ii) Scroll down to find the "GitHub Pages" section and click on the link to redirect to the GitHub pages panel  
iii) Make sure the source is selected to "main"  
iv) Click "Choose Theme" which should redirect to a page that displays the different types of themes available  
v) Choose your desired theme and click "Select Theme"  
vi) Scroll down and press "Commit Changes"  
vii) Open a web browser and type in "\<YOUR USER NAME\>.github.io", to view your resume on a static website  


![AnimatedGif](https://media.giphy.com/media/eLSfc5a1vWQ9KyJDQu/giphy.gif)


### More Resources
* [MarkDown Tutorial](https://www.markdowntutorial.com/)  
* [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) by Andrew Etter  
* [GitHub Pages](https://pages.github.com/)  


Authors and Acknowledgments: This document was written Farhan Akib Rahman, using Andrew Etter's book *Modern Technical Writing* as reference. Reviewed by  

### FAQs

1) Why is my resume not displaying the theme I selected?  
If the markdown file is not written in Git Hub Flavored format the system will not render it accurately, which will cause the website to look different and the theme to not show up.

2) Do I have to use GitHub to host my static webpage?  
No, a static site can be manually hosted by using a generator like Jekyll or Sphinx, by providing a lightweight markup and a theme. The site can be updated by editting the content and processing everything again.  









