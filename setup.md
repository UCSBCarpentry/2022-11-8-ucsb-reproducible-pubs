---
title: Pre-workshop Setup
---

> ## Logging into the RStudio Jupyter Hub Instance
> 
For this workshop, we will be using a Jupyter Hub Instance that LSIT has gracously setup for us with the software and packages preinstalled. <br>
Please use your UCSB NETID to sign into the Jupyter Hub at: [https://carpentryworkshop.lsit.ucsb.edu/](https://carpentryworkshop.lsit.ucsb.edu/) 
Once you have signed in, click the RStudio Launcher button.
**You do not need to follow the setup instructions below if you plan on using the Jupyter Hub Interface rather than RStudio on your own computer**
{: .prereq}

![jupyter-instance](/fig/setup-jupyter-instance.PNG)

> ## Manual Install Requirements
>
If you are **NOT** using the Jupyter Hub instance, and want to use RStudio on your own computer, please follow the instructions below:
{: .prereq}


<h3>PART I: Install Software</h3>

- Github account (use existing or create new account) 
- Install Git for Windows (Windows users only) 
- Install R & RStudio (Two separate installations)

See instructions below for these requirements:

{% include install_instructions/github.html %}

{% include install_instructions/git.html %}

{% include install_instructions/r.html %}

{% include links.md %}



<h3>PART II: Install Packages in Rstudio</h3>

Install the following packages in RStudio: `bookdown`,`quarto` `tidyverse`, `rticles`,`BayesFactor`, `patchwork` , `rprojroot`. 
We will be covering the purpose of using packages and recap different ways to install and manage them in RStudio. Nonetheless, pre-installating the packages we will be using for this workshop will save us some precious time since installation time may vary among learners. Here are the steps for two possible approaches you may follow for completing this process: 

*Using Menus and Tabs*

1) Open R studio
2) Select from the upper menu `Tools > Install packages...` or click on the `Packages` tab in the bottom-right section and then click on install. Either action will prompt a box dialog. 
3) In the `Install Packages` dialog box, copy this command `bookdown, quarto, tidyverse, rticles, BayesFactor, patchwork, here` under the Packages field, make sure the option `install dependencies` is selected, keep other information unchanged, and then click `install`. 
4) Don't be alarmed by the stop sign that will blink (and do not click on it otherwise you will cancel the process) or the red text messages. Once the process completes the cursor will be preceeded by a greater-than sign `>`.

*Entering function in the console*

1) Copy and paste one of the following functions to the console and wait for the process to complete:
~~~

`install.packages("bookdown")
 install.packages("quarto")
 install.packages("tidyverse") 
 install.packages("BayesFactor") 
 install.packages("patchwork")
 install.packages("here")`

~~~
{: .source}
 
 or 

~~~
  
`install.packages(c("bookdown","quarto", "tidyverse", "BayesFactor", "patchwork", "here"))`

~~~
{: .source}

2) Don't be alarmed by the stop sign that will blink (and do not click on it otherwise you will cancel the process) or the red text messages. Once the process completes the cursor will be preceeded by a greater-than sign `>`.

You may close RStudio and all packages will remain installed when you reopen it. 

