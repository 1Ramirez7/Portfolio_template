# Instructions to editing this Portfolio

The main goal of this instructions is focused around editing the _quarto.yml and the process of pushing to github for the site to render. If you follow the steps below on adding new files and editing the _quarto.yml your site should always render. I do not focus to much on the QMD details as that is one of the main concepts we have been working on in class. So you can edit the QMD files as you see fit, and as long as they render locally, they will be published to the site. 




The following are instructions to edit this portfolio separated into sections. Each section is intended to show how to add and or edit different parts of the portfolio. 

# Adding a New Tab

**Adding a new tab to the portfolio.** I’m adding a resume.

1.  In the `_quarto.yml` file add, under the navbar, and this two lines of code\
    `text: "My Resume"`\
    `file: resume.qmd`

2.  Add/create the `resume.qmd` file to the root folder

    -   Render the `resume.qmd` file

3.  Update yml links

    -   Build \> render website

4.  Push to GitHub and the site should be updated with your new tab.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3b-PdI4lhbc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen>

</iframe>


# Adding a Project Tab with Multiple Files

Step 1:  
Adding a tab with a sidebar for multiple QMD files  
- Add tab code to navbar and sidebar code to `_quarto.yml`  

Step 2:  
- Add QMD for the main tab  
- Add a folder with QMD files for the main tab  

<iframe width="560" height="315" src="https://www.youtube.com/embed/ansNLTE6yms" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen>

</iframe>



# Working with Python Code & Environment in R-Studio

Part 4. Working with Python code, environment, and `requirements.txt` files in R-Studio  

**Step 1:** Check what environment is active (likely a global environment)  
`library(reticulate)`  
`py_config()`  

**Step 1.7:** Create a virtual environment if needed (basically needed in any new device)  
`library(reticulate)`  
`virtualenv_create("env")`  

**Step 1.5:** Load environment for the project if needed. Use the code from Step 1 to make sure the new environment is loaded. If not, use this to load the new environment. Replace `env` with the actual name of your environment.  
`library(reticulate)`  
`use_virtualenv("env", required = TRUE)`  

**Step 2:** Install Python libraries  
`library(reticulate)`  
`py_install(c("pandas", "numpy", "matplotlib"))`  

**Step 2.1:** Run Python code/file and render Python files  

**Step 3:** Create/update the `requirements.txt` file  
`shell("pip freeze > requirements.txt")`  

<iframe width="560" height="315" src="https://www.youtube.com/embed/rrsIChN1H1c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/gvebioDsuAg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
