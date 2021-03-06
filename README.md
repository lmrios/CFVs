# GUI to control a test rig with Critical Flow Venturies
Since this is a private project, there will be a only a small working part of it.

Critical Flow Venturies (CFVs) are an excellent reference for mass flow.
However CFVs are modeled by fluid mechanics equations which are complex and non linear. 
I think,  if we can find a new model using Neural Networks maybe we can predict how the model will behave at different inlet pressures.

This program plots in real-time the received data on a embedded graph.
Up to now it uses:
- Python3
- PyQt5

###  Results presented at AFA 2017
There is a Poster - in PDF  format -  presented at the poster session at AFA 2017. 
https://github.com/lmrios/CFVs/blob/master/PosterAFA2017CFVs.pdf <br/>
I am sorry poster is in Spanish. There will be a English version SOON. <br/>
It is possible to see the on the Results section that Figure 4 and Figure 7 on the poster shows some minor differences with NIST - USA Calibration.
We are fixing this, after that the code will be uploaded.

### Preview
Here is what it looks like: 
![preview](imgs/PreviewCFVs_1.PNG?raw=true "Preview of the GUI for the CFVs ")

### Tip
Remember to do this for the images.

Type in the console this "compile" the ui file to python, with this command:
pyuic5 -x UInozzles2018.ui -o codeUInozzles2018.py

An the same goes to the "ResourceImgFile.qrc" file a python, with this command:
pyrcc5 ResourceImgFile.qrc -o codeResourceImgFile.py

Note: codeResourceImgFile.py will be import from codeUInozzles2018.py, so check the import lines ;)