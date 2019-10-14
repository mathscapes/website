---
layout      : post
title       : Linking ABAQUS and FORTRAN
author      : Rahul Singh
tags        : ["ABAQUS", "FORTRAN", "Vumat", "FEM", "Tutorial" ]
cite        : true
---

ABAQUS and FORTRAN are linked to execute user subroutines such as VUMAT, UMAT, USDFLD, etc. 
You can find various versions of ABAQUS and FORTRAN Available. Here is the compatibility list:
- ABAQUS 2017
- Intel Composer XE 2013 or above 
- Visual Studio 2010 or above v6.14
- Intel Visual Fortran 12.0 or above 
- Visual Studio 2010 or above

One can download Student version of FORTRAN for free from [here](https://software.intel.com/en-us/qualify-for-free-software/student).

## Step 1. Installation
Install your copy of SIMULIA ABAQUS followed by Visual Studio and Visual Fortran. Make sure you install C++ component of Visual Studio as well.

## Step 2. Fortran Compiler
Find `ifort.exe` and `ifortvars.bat` in Installation directory of FORTRAN. Copy the address on clip board.

```
"C:\Program Files (x86)\Intel\Composer XE 2013 SP1\bin\ifortvars.bat" intel64 vs2012
```

![]({{ site.baseurl }}/assets/images/abaqus_link1.png)


## Step 3. Visual Studio
Go to Installation directory of Visual Studio and copy the address of `vcvarsall.bat`.

```
"C:\Program Files (x86)\Microsoft Visual Studio 11.0\VC\vcvarsall.bat" x64
```

![]({{ site.baseurl }}/assets/images/abaqus_link2.png)

## Step 4. Including Directories in ABAQUS CAE

Go to Installation directory of ABAQUS and find `launcher.bat`.

Open the file with notepad and paste the addresses in the following manner:

![]({{ site.baseurl }}/assets/images/abaqus_link3.png)

Same can also be done by right-clicking on ABAQUS CAE shortcut → Open File Location

Save the file.

## Step 5. Run ABAQUS Verification

Run ABAQUS Verification first, It'll create a `verify.log` opening which you can check if the procedure was successful.

![]({{ site.baseurl }}/assets/images/abaqus_link4.png)

## Step 6. Run ABAQUS CAE

Click and open ABAQUS, you will be able to see that FORTRAN is also called along with it.

![]({{ site.baseurl }}/assets/images/abaqus_link5.png)