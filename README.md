# YSIG

## To obtain the code written by the Macro/Systematic Strategies group, follow the instructions below.

#### Instructions for Mac users

Open Terminal and type "python --version" into the command prompt. Your python version should be 3.0 or greater for compatibility with our code. Otherwise, you need to download a more recent version of python. I recommend that you install the Anaconda python distribution, which can be found at https://www.continuum.io/downloads.

Make sure that you have developer tools installed. You can install by running the following line:

xcode-select --install

If you do not already have a github account, create one at www.github.com.

Once you create an account, type "git --version into the command prompt. If you do not have git installed, go to https://git-scm.com/downloads and download git.

Next, confirm that you have collaboration permissions for the systematic_investment and systematic_analyses repositories. If you have not received an email invite, send an email to david.adelberg@yale.edu requesting an invitation.

You'll have to setup git large file storage. Execute the following:

brew install git-lfs

git lfs install

In the command prompt, navigate to the directory where you would like to store the downloaded files (the cd, ls and mkdir commands will be useful for this.) Then, execute the following:

git clone https://github.com/david-adelberg/YSIG.git

git clone https://github.com/david-adelberg/systematic_investment.git

git clone https://github.com/david-adelberg/systematic_analyses.git

cd systematic_investment

python setup.py develop

This code will download the files in the YSIG, systematic_investment and systematic_analyses repositories. YSIG contains general YSIG documents. The systematic_investment repository contains a package to accelerate the development of systematic investment models. systematic_analyses contains the models we are working on.

You are done! To make sure that everything was set up correctly, open your favorite python IDE, open the systematic_analyses project and run SPDefinitions.py. This should run a simple statistical model that aims to predict the S&P 500 for the next year.

If you downloaded Anaconda, you can click on the Navigator and then open Spyder. In the project explorer, click on the blue folder and choose the systematic_analyses folder. Then double click on SPDefinitions.py and click the green arrow in the upper left corner to run the file.

