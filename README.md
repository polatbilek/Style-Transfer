# Style-Transfer
Image Style Transfer Model which re-creates the content image with the painting style of the style image.

## Run
### Installing Packages
To get the code execute the command below on your terminal.
`git clone https://github.com/polatbilek/Style-Transfer.git && cd Style-Transfer`

This code works on python3, so you need python>=3.5.
To install packages you need to install pip or pip3 (depends on your PC's config).
You need to execute commands below to get required packages (pip or pip3, the on who installs to python3 env.)

`pip install IPython`
`pip install pillow`
`pip install matplotlib`
`pip install tensorflow`

### Execution
At the end of the code, you will a code snippet like shown below:

`# Only adjusting these parameters enough`
`  content_path = '/path/to/your/photo.jpg'`
`  style_path = '/path/to/your/style_photo.jpg'`
`  content_weight = 1e3 # default 1e3`
`  style_weight = 1e-2  # default 1e-2`
`  iteration = 1000     # must be divisible by 100`
  
You need to set the paths first, then you can adjust parameters to get required type of image. Higher style_weight loose content but apply the style more, and more content_weight protects the content with less and less style. More iteration is better but below 700 is not recommended, also no need to go higher than 1300 (nothing changes above that).

To run the code execute the code below (it takes approximately 1 hour to finish, you can save the output image after finishing)
`python3 style.py`
