---
title: FEFF
---

# Downloading FEFF

To obtain FEFF, first fill out the registration form [Here](https://times-software.github.io/feff10/)

Once you have registered, you will receive a download link along with a copy of the installation instructions.


# Instructions for setting up JFEFF+FEFF10

## Windows:

1.  You need an updated version of java for JFEFF to work. Please [install java](https://www.java.com/download/ie_manual.jsp) if it is not already installed. 
    
2.  Go to the [feff10 releases page](https://github.com/times-software/feff10/releases/latest) and download **jfeffv9.x.x_feffv10.x.x_win_installer.exe**, and run the installer.
    
3.  Open jfeff.
    
4.  Click on "Settings" in the lower right corner.
    
5.  Click on "Browse" next to "Feff Module Dir".
    
6.  Browse to "your\_install\_directory\\JFEFF\_FEFF10\\feff10\\bin" and click "Open". For most people "your\_install\_directory" is "C:\\Windows\\Program Files (x86)"
    
7.  Click OK.
    
8.  You can now try running the pre-loaded example by clicking "Save and Run" in the lower right hand corner.
    
9.  The calculation should only take a few seconds. Once it is done, you can plot the results by clicking "Plot" in the lower right hand corner.
    
10.  You can find examples in your home directory in a directory named "feff10\_examples". Note that some of these examples do not work with JFEFF, although all should work with FEFF10.
    

## Mac:

1. If you have a mac with M1 or M2 chip rather than Intel, you will need to install rosetta. To do so, open a terminal and type the following command: 
`/usr/sbin/softwareupdate --install-rosetta --agree-to-license`
Hit enter to agree and install.

2. In order to install JFEFF+FEFF10 on OSx, you will need java jdk 8, which you can find at [JDK8 Download](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html). Choose the macos x64 file.
    
3. Download jfeffv9.x.x\_feffv10.x.x\_osx\_install.tgz from the [FEFF10 Download page](https://github.com/times-software/feff10/releases/latest)
    
4.  Open a terminal. Note that when you run some of the following commands, you might see a message: "Terminal would like to access files in ..." If you see this message, click "OK"
    
5.  Change directories to the location of the downloaded install file. For example, 
`cd Downloads`
    
6.  Extract the install directory: 
`tar -zxvf jfeffv9.x.x\_feffv10.x.x\_osx\_install.tgz`
    
7.  Move to the jfeffv9.x.x_feffv10.x.x_osx_install directory. 
`cd jfeffv9.x.x\_feffv10.x.x\_osx\_install`
    
8.  Run the installer 
`./jfeff\_installer.sh`
    
9.  NOTE: Users of OSx Catalina and Big Sur may see the message: "jfeff_feff10.0.0_osx_install cannot be opened because the developer cannot be verified." If you see this message, click "Cancel" and run the following commands: 
`cd .. ; xattr -rd com.apple.quarantine jfeffv9.x.x\_feffv10.x.x\_osx\_install ; cd jfeffv9.x.x\_feffv10.x.x\_osx\_install` Now run the installer as specified above in step 8.
    
10.  Follow the directions to install jfeff.
    
11.  Run jfeff - Browse to the directory you specified during installation, and double click on "jfeff10.app" Alternatively, run jfeff from the command line by typing: `open your\_home\_directory/jfeff10.app`
    
12.  You will see a message about copying files. Click "Don't Copy Files"
    
13.  Click on "Settings" in the lower right corner.
    
14.  Click on "Browse" next to "Feff Module Dir".
    
15.  Browse to "your\_install\_directory/jfeff10.app/Contents/Resources/JFEFF/feff10/mac/" and click "Open".
    
16.  Click "OK"
    
17.  You can now try running the pre-loaded example by clicking "Save and Run" in the lower right hand corner.
    
18.  The calculation should only take a few seconds. Once it is done, you can plot the results by clicking "Plot" in the lower right hand corner.
    
19.  You can find examples in your home directory in a directory named "feff10\_examples". Note that some of these examples do not work with JFEFF, although all should work with FEFF10.
    

## Linux:

1.  In order to install JFEFF+FEFF10 on linux, you will need Oracle java, which you can find at [https://www.java.com/en/download/](https://www.java.com/en/download/)
    
2.  Download jfeffv9.x.x\_feffv10.x.x\_linux\_install.tgz from the [FEFF10 Download page](https://github.com/times-software/feff10/releases/latest)
    
3.  Open a terminal.
    
4.  Change directories to the location of the downloaded install file. For example, 
`cd Downloads`
    
5.  Extract the install directory: 
`tar -zxvf jfeffv9.x.x\_feffv10.x.x\_osx\_install.tgz`
    
6.  Move to the jfeffv9.x.x_feffv10.x.x_osx_install directory. 
`cd jfeffv9.x.x\_feffv10.x.x\_linux\_install`
    
7.  Run the installer 
`./jfeff\_installer.sh`
    
8.  Follow the directions to install jfeff.
    
9.  Run jfeff 
`your\_home\_directory/JFEFF\_FEFF10/jfeff10`
    
10.  You will see a message about copying files. Click "Don't Copy Files"
    
11.  Click on "Settings" in the lower right corner.
    
12.  Click on "Browse" next to "Feff Module Dir".
    
13.  Browse to "your\_home\_directory/JFEFF\_FEFF10/feff10/linux/" and click "Open".
    
14.  Click "OK"
    
15.  You can now try running the pre-loaded example by clicking "Save and Run" in the lower right hand corner.
    
16.  The calculation should only take a few seconds. Once it is done, you can plot the results by clicking "Plot" in the lower right hand corner.
    
17.  You can find examples in your home directory in a directory named "feff10\_examples". Note that some of these examples do not work with JFEFF, although all should work with FEFF10.
