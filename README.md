# How to Host a Resume in Markdown Format With Github Pages
## Purpose
Describe how to format a resume using Markdown and host it using Jekyll and Github Pages. The steps will be based on some general principles of technical writing as described in **Andrew Etter's** book _Modern Technical Writing_.

## Prerequisites
* A Github Account
* A resume formatted in Markdown
* Markdown Editor

Refer To the **"More Resources"** section in case you need further information.

## Instructions

Andrew Etter mentioned some of the benefits of using distributed version control in his book _Modern Technical Writing_. Github is a distributed [versin control system](https://www.atlassian.com/git/tutorials/what-is-version-control#:~:text=Version%20control%2C%20also%20known%20as,to%20source%20code%20over%20time.) that allows multiple users/developers to collaborate on the same files and therfore help teams to manage changes to source code over time.

### Setting up a New Github Repository
*  Log in into your [Github](https://github.com/) Account.
* Select New repository from the drop-down menu in the upper-right corner of any page.
* Name your repository in the follwoing way in order for the Github Pages to recognize your repository.
```[your-username].github.io```
* Choose the repository's visibility to be **Public**.
* Do not add the initial README.
* Click **Create repository**.

### Add Files to the Repository using GitHub Account
* Go to the desired repository.
* Click **add file** on the top right of the repository menu.
* Create two files named index.md and README.md. 
* Copy your markdown formatted resume and README into index.md and README.md respectively.

### Add/Edit Files in the Repository Using a Local Repository

* Go to the desired repository and copy the [HTTPS-link] under the **code** menu at the top right.
* Open a command terminal on your computer and navigate to the desired directory.
* Create a local copy of your repositoy using-
```git clone [Https-link]```
```git checkout -b [branch-name]```
* Add or edit the index.md and and README.md files under the local folder created.
* Push the changes to the remote Github Repository by following these steps-
```Git add .```
```Git commit -m "message"```
```Git push origin [branch-name]```

Refer To the **"More Resources"** section in case you need further information about how to use ***Git***.

### Setting up GitHub Pages
Since our repository has been setup, now we have to pick a theme and host our resume on GitHub Pages which deploys a static website containing our resume.

According to Andrew Etter, static websites are very easy to use; they don't require a connection to a server-side programme or database, and there is less chance of problems. They are simple to create and are ideal for activities when the only thing displayed is text, such as documentation.

* **Pick a Theme**   
    *  Navigate to Settings>Pages>Theme Chooser.
    * Select a preferred theme and click **save**.
    * A new file named _config.yml will be created in the main repository. GitHub Pages generates static sites from markdown files using the Jekyll framework. This config file is used by Jekyll to choose which theme to apply.

* **Change the Title of Your Website**
    * To change the title of your static site edit config.yml generated in the gh-pages branch and add the line
    ```title: "[my-title]" ```

## Results
* Navigate to Settings>Pages.
* Click on the link to your published static website.

You can also access the site by typing the following URL into the address box. It should be something along the lines of ```https://[Username].github.io/```.

## More Resources
[_Modern Technical Writing_ by Andrew Etter]( https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
[Markdown Tutorial](https://www.markdowntutorial.com/)  
[Git Tutorial](https://www.w3schools.com/git/)  
[Jekyll Documentaion](https://jekyllrb.com/docs/) 

## Authors and Acknowledgments   
* **Author**: Jishan Arora 
* **Group Members**: 
    * Jishan Arora
    * Xing Zhou
    * Tanisha Turner
    * Adam Donen

## Frequently Asked Questions
* Why are we using Markdown?   
    * Markdown is superior to word processors in that it is easy to learn, customise, and read for both humans and machines. It may also be written and modified in practically any editor on almost any platform, making it extremely portable.
* Why is my resume not showing?
    * Make sure that the name of the repository and the files mentioned are correct as GitHub Pages can cause errors incase the name of the files doesn't match with the given format.



