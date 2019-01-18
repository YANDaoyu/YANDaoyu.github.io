---
layout: post
title: "Marks of Lesson: Python Scientific Computing 3D Visualization"
author: "Island"
categories: NetLesson
tags: [Python]
---

From 1st, June, 2018 to ...

[Python Scientific Computing 3D Visualization](https://www.icourse163.org/learn/BIT-1001871001?tid=1002856007), Tianyu HUANG, Tian SONG, BIT, MOOC.

## Environmental preperation for the lesson

Me: Windows 10, Visual Studio Code, Anaconda3(64-bit), VTK 8.1.0

Need: TVTK - from mayavi package (installed in week 01).

### Installation TVTK

TVTK is meant to be installed as part of the `mayavi` package. Please visit the installation guide on the [Mayavi documentation](http://docs.enthought.com/mayavi/mayavi/installation.html). This document only covers building and using TVTK from inside a checkout of the the mayavi repository.

So I tried to do "conda install mayavi" in `Anaconda Prompt` but...????

```bash
(base) C:\Users\Username>conda install mayavi
Solving environment: failed

UnsatisfiableError: The following specifications were found to be in conflict:
  - mayavi -> apptools==4.2.0 -> python=2.7
  - python=3.6
Use "conda info <package>" to see the dependencies for each package.
```
So I install `apptools`, but... install traits-4.6.0 by this call.

```bash
(base) C:\Users\Username>conda install apptools
Solving environment: done

## Package Plan ##

  environment location: E:\Anaconda\Anaconda3

  added / updated specs:
    - apptools


The following packages will be downloaded:

    package                    |            build
    ---------------------------|-----------------
    configobj-5.0.6            |           py36_0          53 KB
    apptools-4.4.0             |           py36_0         395 KB
    certifi-2018.4.16          |           py36_0         143 KB
    traitsui-6.0.0             |           py36_1         866 KB
    traits-4.6.0               |           py36_0         412 KB
    conda-4.5.4                |           py36_0         1.0 MB
    pyface-6.0.0               |           py36_0        1019 KB
    ca-certificates-2018.03.07 |                0         155 KB
    openssl-1.0.2o             |       h8ea7d77_0         5.4 MB
    ------------------------------------------------------------
                                           Total:         9.4 MB

The following NEW packages will be INSTALLED:

    apptools:        4.4.0-py36_0
    configobj:       5.0.6-py36_0
    pyface:          6.0.0-py36_0
    traits:          4.6.0-py36_0
    traitsui:        6.0.0-py36_1

The following packages will be UPDATED:

    ca-certificates: 2017.08.26-h94faf87_0                  --> 2018.03.07-0
    certifi:         2017.7.27.1-py36h043bc9e_0             --> 2018.4.16-py36_0
    conda:           4.5.0-py36_0               conda-forge --> 4.5.4-py36_0
    openssl:         1.0.2n-vc14_0              conda-forge [vc14] --> 1.0.2o-h8ea7d77_0

Proceed ([y]/n)? y


Downloading and Extracting Packages
configobj 5.0.6: ############################################################################################## | 100%
apptools 4.4.0: ############################################################################################### | 100%
certifi 2018.4.16: ############################################################################################ | 100%
traitsui 6.0.0: ############################################################################################### | 100%
traits 4.6.0: ################################################################################################# | 100%
conda 4.5.4: ################################################################################################## | 100%
pyface 6.0.0: ################################################################################################# | 100%
ca-certificates 2018.03.07: ################################################################################### | 100%
openssl 1.0.2o: ############################################################################################### | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
```

But when I recall "conda install mayavi", the result just as same as it before.

So, BYEBYE CONDA. I return to pip install, call "pip install mayavi" and then success.

Let's test a [demo](https://zhuanlan.zhihu.com/p/28051202).