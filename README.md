# Assignment 1

## Part A: Installation & Account Setup

In this assignment you will be setting up the software and online tools that you will be using throughout this course. Below there are links and instructions to relevant sites.

The first step is to create a [Github account](https://github.com/join?source=header) if you do not already have one: 

Next you will need to install the software we will be using (if you already have them installed make sure they are the latest versions):
   * R
   * RStudio
   * Git
   * Swirl Package in R
   
## Installing R
* Choose a [download mirror site](https://cran.r-project.org/mirrors.html) from the list that is close to you geographically  
* Download the version of R that is appropriate to your operating system
* Install R in a manner appropriate to your operating system ([MacOSX](https://youtu.be/Ywj6yNfc5nM), [PC](https://youtu.be/5ZbjUEg4a1g))

## Installing RStudio (Graphical User Interface for R)
* Download the free version of [RStudio](https://www.rstudio.com/products/rstudio/download/)
* Install RStudio in a manner appropriate to your operating system ([MacOSX](https://youtu.be/Ywj6yNfc5nM), [PC](https://youtu.be/5ZbjUEg4a1g))

## Installing Git
* Git is a version control system to keep track of our work and collaboration
* Instructions for setup can be found [here](https://help.github.com/articles/set-up-git/) and [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* Download [Git](https://git-scm.com/downloads) 

## Connecting Git-Github-RStudio
* You will also need to link your Github account to RStudio by following [these instructions](https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN) or [these instructions](http://happygitwithr.com/rstudio-git-github.html).
* For many students this will be the most challenging task this semester. Several errors can be corrected by following the instructions located [here](http://happygitwithr.com/troubleshooting.html).

A common error is: 

`error: unable to read askpass response from 'rpostback-askpass'`

The fix for most systems is:

* In RStudio, click on the "Tools" menu and select "Shell"
* Run the following command: `git push -u origin master` (*it might ask you for your git username and password. Supply this information, make sure it is correct*)
* Close the window
* Now make some more edits to some file so that you have new content to push click on the "push" button in RStudio and this time the push should work

If you are using a Mac and this does not fix your error please try [these instructions](https://github.com/core-methods-in-edm/Assignment1/blob/master/MAc%20Github%20help%20pages.pdf). 

## Part B: Swirl

* Once you have installed both programs, open RStudio (RStudio will automatically open R at the same time)
* R is modular, we can install mini-programs called *packages* within it like apps on your phone to do specific tasks, in this activity we will be using the Swirl package. Swirl is a teaching tool for learning R, it comprises questions and answers and a bit of AI (for positive reinforcement)
* Install the Swirl package by typing `install.packages("swirl")` in the console window (located on the left hand side of the RStudio interface). If you get an error message you can also install by clicking the "packages" tab in the right hand pane and then clicking "install".
* Once we have installed the package we need to turn it on, we do this by inputing the code `library(swirl)` - Swirl will tell you to type `swirl()` **but don't do that just yet!**
* First we need to load a lesson into Swirl, to do this cut and paste the following code into the console window (you will need to be connected to the internet):  
`install_course_github("core-methods-in-edm", "swirl", multi = TRUE)`
* Once the lesson finishes installing type `swirl()`, Swirl will then guide you through setting up a user Id (please use your full name so we can identify you later). Choose the `Unit 1 - Introduction` course and the `Basic Building Blocks` lesson when you have the option.
* At the completion of the lesson you will submit your answers through a Google form. We will collect information on how many questions you answer, how many attempts you took to answer each question and the time you answered

## Part C: R Markdown

The final part of this assignment is for you to utilize all the software you just installed to modify an R Markdown file.

* In the top left corner of the repository page, click `Fork` - this step is often forgetten, try not to forget it!
* Then click `Clone` and copy the URL for the repository
* Open RStudio and click `File` -> `New Project` -> `Version Control` -> `Git`
* Paste the URL into the `Repository URL` box
* Name your project in the `Project Directory Name` box
* Browse to an appropriate folder on your computer to put your project, I would suggest you make a folder for the class somewhere, don't put the project on the Desktop or in the Root Directory. Moving a project after you create it can cause problems later so it is best to put projects somewhere that is permanent.
* Click `Create Project`
* Once you have created your project open the `Assignment1.Rmd` file by clicking on it in the `Files` pane of RStudio (bottom-right by default)
* Open the `R Markdown Cheat Sheet` also available under `Files` 
* Use the Cheat Sheet to make the following changes to the Assignment1.Rmd file:
  * Create a top level heading that says "Assignment 1"
  * Insert a link to your Github profile page
  * Create a second level heading that says "My Goals for HUDK4050"
  * Create a bulletted list that describes three goals you have for this class
  * Create another second level heading that says "Video Review"
  * Create a table with two columns and three rows. In the header (first row) of the first column put the word "Category", in the header of the second column put the word "Review". In the second row of the first column put the word "Change" and in the third row of the first column put the word "Keep". In the remaining two cells write your opinion of the class videos you have seen so far. Wite a sentence or two about what you would change in the second row and what you would keep in the third row.
  * Create another second level heading that says "This is how I am feeling about the semester"
  * Find an image of a piece of art that sums up how you are feeling about the semester ahead, upload it to the repository (add it to the folder where your project is located) and then insert it into the document
* Now look of the Git icon in RStudio - top right tab or top left pane - and click it
* Click `Commit`
* In the left hand pane click the boxes for your `Assignment1.Rmd` file and your image file
* Write a message in the `Commit Message` box, something that describes the work you have done like "Uploading assignmnet 1 .Rmd file"
* Click `Commit`
* Click `Push`
* Now return to Github and refresh the page, your edited .Rmd file and your image file should now be in the repository
* Next, to submit your assignment click `Pull Requests`and then `Create New Pull Request` 


