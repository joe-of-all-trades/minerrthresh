# minerrthresh

Poisson distribution-based minimum error thresholding

thresh = minerrthresh(img) returns minimum error threshold for the input image
thresh = minerrthresh(img,'Gaussian') will use Gaussian instead of Poisson model in determining the threshold
thresh = minerrthresh(img,'bin',num) will use the bin number specified by num instead of the default, 128
[thresh, stats] = minerrthresh(img) will also return stastistics including the alpha values and prior probablities for foreground and background 
---------------------------------------------------------------------------
This function is adapted from the C++ code published in 
Yousef Al-Kofahi et al, Improved Automatic Detection and Segmentation of
Cell Nuclei in Histopathology Images. IEEE Transcations on Biomedical
Engineering, Vol 57. No 4, April 2010

This is Pal and Bhandari modified version of minimum error thresholding 
first propsed by Kittler and Illingworth. The original Kittler and 
Illingworth version assumed Gauassian distribution while Pal and Bhandari 
used Poisson distribution instead.

2015 Chaoyuan Yeh
