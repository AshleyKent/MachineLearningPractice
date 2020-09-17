###### This respository will be using code modified from https://github.com/vivekhsridhar/tracktor. This was the first machine learning software that I found when trying to understand more about using OpenCV. It is software intended for those with basic coding/scripting skills to be able to utilize. I will be walking through the steps and writing notes indicating how I utilizes this software and any issues that I have encountered as well as how those issues were resolved. These steps are detailed in the walkthrough on Tracktor's Github in much more detail so please check that out. It is a wonderful resource.

Installation Process
--------------------

#### A. Downloaded miniconda at https://docs.conda.io/en/latest/miniconda.html
This was pretty straightforward and I didn't have any problems using it.

#### B. Created and activated a virtual enviornment in miniconda

Using the Anaconda prompt, I typed:
'conda create --name myenv'
(I replaced "myenv" with an appropriate name)

Then I confirmed the selection in ('proceed ([y]/n)?), by typing 'y',

Then I activated the environment that I just created by typing 'activate myenv' (windows)

#### C. Installed necessary python packages

Typed 'conda install pip' to get the pip installer running in my activated environment

Installed the following packages
  • 'pip install numpy'
  • 'pip install pandas'
  • 'pip install scipy'
  • 'pip install scikit-learn'
  • 'pip install matplotlib'
  • 'pip install ipython'
  • 'conda install ipykernel; (Pip had difficulty so I had to use conda for this command)
  • 'pip install jupyternotebook'
  
Created a 'kernel' for my virtual environment by typing:

'python -m ipykernel install --user --name myenv --display-name "python (myenv)"'

### D. Installed OpenCV

I had some difficulty with this but eventually I was able to get it to work by typing:

'pip install opencv-contrib-python'

Tested to make sure it worked by typing 

'python'
'import cv2'

I had no problems with this part so I typed "exit()

### E. Downloading Tracktor

You actually only have to download the tracktor.py but it is suggested for unexperienced users to use the jupyter notebook examples and change the parameters. 
