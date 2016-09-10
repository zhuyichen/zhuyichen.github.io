---
layout: post
title:  BAYOMA APP OVERVIEW
date:   2016-09-10 16:02 +0100
categories: BAYOMA
---
The BAYOMA app for iOS is designed to have the following functions:

- Manage the vibration data file
- Record vibration data
- Plot time history data; PSD and SV spectrum
- Rough Estimation of modal Parameters
- Bayesian modal identification (BAYOMA)

## Manage the vibration data file

Class used: NSFileManager [Examples from NSHipster][NSFileManager-NSHipster]

## Record vibration data

Class used: CMDeviceMotion [Examples from NSHipster][CMDeviceMotion-NSHispter]
More Examples: [Apple Dev Doc][CoreMtion-apple] [iOS加速度数据获取][jianshu]

## Plot time history data; PSD and SV spectrum

Library used: [Charts][charts] from Github

## Rough Estimation of modal Parameters
Based on pick peaking, half bandwidth and eigenvector method, the natural frequency, damping ratio and mode shapes can be roughly estimated within Objective C (NSObject Class).

## Bayesian Modal identification

Using MATLAB Coder, the MATLAB functions can be transferred to C/C++ code or shared library (.dll file)

References: [MATLAB Coder的使用][useageofmatlabcoder]

Attention: some functions can not be transferred so it should be rewritten (e.g. cell,cell2mat, eigs).




[NSFileManager-NSHipster]: http://nshipster.com/nsfilemanager/
[CMDeviceMotion-NSHispter]:http://nshipster.com/cmdevicemotion/
[CoreMtion-apple]:https://developer.apple.com/reference/coremotion
[jianshu]:http://www.jianshu.com/p/53ae8023a9ea
[charts]:https://github.com/danielgindi/Charts
[useageofmatlabcoder]:http://chunqiu.blog.ustc.edu.cn/?p=898
