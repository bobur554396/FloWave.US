# FloWave.US
FloWave.US is a MATLAB program for automated ultrasound blood flow analysis. FloWave.US extracts blood velocity and vessel diameter from ultrasound screen captures, giving researchers the flexibility to calculate a variety of vascular health parameters. 

## Resources
- [Journal of Applied Physiology Reference] (http://jap.physiology.org/content/121/4/849 "Journal of Applied Physiology Reference")
- [Instruction Manual] (https://github.com/ccoolbaugh/FloWave.US/tree/master/Documentation "Instructions") (Wiki coming soon)
- [Example Videos] (https://github.com/ccoolbaugh/FloWave.US/tree/master/Demo "Demo Videos")
- [Release Notes] (https://github.com/ccoolbaugh/FloWave.US/releases "Release Notes")
- [Getting Started with MATLAB] (http://www.mathworks.com/help/matlab/getting-started-with-matlab.html "MATLAB Help")

## Installation
Assumes MATLAB (release 2011b or newer) installed:  

1. CLICK the green "**Clone or download**" button.   
2. SELECT the "**Download ZIP**" option to download the latest program release.   
3. SAVE the unpacked source code files into a folder directory of your choosing.  
4. OPEN **MATLAB** and set the working directory to the location of your downloaded files.   
5. TYPE `FloWaveUS` into the MATLAB command prompt to run the program. 
  * Assumes an ultrasound screen setup file exists - see the next section for more details.  

If you have any installation problems, please file an [issue] (https://github.com/ccoolbaugh/FloWave.US/issues "Issues") with a description of your problem, and we will try to help you. 

## Custom Ultrasound Screen Setting Files
*FloWave.US* requires an ultrasound screen setup file to adapt the program to different ultrasound scanners and operation modes. To create a screen setup file: 

1. OPEN **MATLAB** and set the working directory to the location of your downloaded files.  
2. TYPE `UsSetup` into the MATLAB command prompt and follow the on-screen instructions.  
3. SAVE the ultrasound screen setup file (e.g. "SETUP.mat") in the same working directory for easy access.  

## Video Recording Requirements
*FloWave.US* analyzes digital video recordings of duplex or brightness mode (B-Mode) ultrasound screen captures. For the best results, the screen capture should meet the following requirements:  

* **High Definition Acquisiton**: video recordings of the ultrasound screen should be acquired at a mininmum sampling rates of 30 frames per second. Video recording equipment can typically be connected to the ultrasound scanner's video output or composite output port.  
  * Example Recording Equpiment:  
    * [Sony DVD Recorder (VRD-MC6)] (https://esupport.sony.com/US/p/model-home.pl?mdl=VRDMC6 "Sony DVD Recorder")  
    * [Startech Video Capture Device (USB3HDCAP)](https://www.startech.com/AV/Converters/Video/usb-3-0-video-capture-device-hdmi-dvi-vga~USB3HDCAP "Startech USB")  
* **View of On-Screen Scales**: screen captures must include the manufacturer's calibration scales (e.g. velocity, distance, time) to convert pixels into the units of interest. These scales should be visible in addition to a complete view of the B-Mode or duplex image.  
* **MATLAB Compatible Video File**: digital video files must be saved/converted to an AVI or MOV format.  
  * Windows 7 or later: AVI or MOV  
  * Macintosh: MOV only  
*  **Removal of On-Screen Calculations/Markings**: on-screen calculations (e.g. cardiac cycle gates) should be turned off during the video recording to avoid obstructing the view of the B-Mode or duplex image.  

## Running the Demo Videos
We have provided [demo videos] (https://github.com/ccoolbaugh/FloWave.US/tree/master/Demo "Demo") to ensure the *FloWave.US* source code works on your computer:  
* **DemoMuscleContraction.mov**: duplex ultrasound video recorded in the lower leg during a 1-s muscle contraction experiment - a test case for the main *FloWaveUS.m* program or to practice creating ultrasound screen setting files with *UsSetup.m*.  
* **DemoBMode.mov**: B-Mode ultrasound video recorded in the upper arm at rest - a test case for the vessel diameter measurement program *BMode.m*.  
* **GELogiqBookeDefault.mat**: ultrasound screen settings file for a General Electric Logiq Book e ultrasound scanner - this file is needed to analyze the muscle contraction demo video. 

## Questions / Feedback?
Have an idea for *FloWave.US*? Found a bug? Please file an [issue](https://github.com/ccoolbaugh/FloWave.US/issues "Bug Reports") on GitHub. 

If you report a bug, please include the following details:  
* *FloWave.US* version number (e.g v.0.2.0)
* Context Information - what you were trying to do when the bug happened? (screen shots can be very helpful)
* Steps to Reproduce the Error - does the error continue to happen in a repeatable manner?

## Contributing
We also encourage community members to write code - you can do so through GitHub by forking the respository and sending a pull request. When submitting code, please try to follow existing conventions and style to keep the code readable.

By contributing your code, you agree to license your contribution under the terms of the MIT License. 

## License
* *FloWave.US* is license under the MIT [license](https://github.com/ccoolbaugh/FloWave.US/blob/master/LICENSE "License").  
* Third-party software (ginputc.m and imgaussian.m) are used according to their respective license agreements.   

## Remarks
Thank you for your interest in *FloWave.US*. We hope the program continues to improve and become a community effort to provide high quality, efficient, and inexpensive data processing solutions for ultrasound blood flow research. 

If you find *FloWave.US* useful in your research, please consider citing the following:  

1. C.L. Coolbaugh, E.C. Bush, C.F. Caskey, B.M. Damon, and T.F. Towse, "FloWave.US: a validated, open source, and flexible software for ultrasound blood flow analysis," *J Appl Physiol*, p. jap.00819.2015; **DOI**: 10.1152/japplphysiol.00819.2015
