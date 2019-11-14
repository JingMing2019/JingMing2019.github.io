---
title: "Circular Array 3D SAR System Simulation and Ground Test Experiment"
collection: researches
permalink: /research/2019-01-31-Circular-Array-3D-SAR-System-Simulation-and-Ground-Test-Experiment
excerpt: 'A new circular array 3D SAR system is presented with Point Spread Function derivation and ground test results which demonstrates its high-resolution imaging ability and effective side-lobe suppression capability.'
datestart: 2018-08-31
dateend: 2019-01-31
venue: 'School of Information and Communication Engineering, UESTC'
program: 'The National Natural Science Foundation of China'
mentor: Prof. Xiaoling Zhang
location: Chengdu, China
---

Background
===
[Circular Synthetic Aperture Radar (CSAR)](/images/rsrch-2019-01-31-1.png) and [Linear Array Synthetic Aperture Radar (LASAR)](/images/rsrch-2019-01-31-2.png) are two kinds of SAR models, capable of 3-dimensional SAR imaging. CSAR can provide multi-angle information, whereas it lies drawbacks of the high image sidelobes due to the sparse sampling in the cross-track direction. LASAR can acquire high-resolution 3D imaging results, so long as the condition of the large-scale linear array and sufficient sampling rate are met, which at present are difficult to realize. 

Therefore, we come up with the idea of combining the geometric structure of both techniques to create a new model equipped with both advantages and compensate for each technique's shortage. [**Circular Array Synthetic Aperture Radar (CASAR)**](/images/rsrch-2019-01-31-3.png) makes the linear array antenna to move in circular trajectory （or drives a single antenna to move in a spiral motion） to effectively increase the sampling rate in the cross-track direction which results in the suppression of image sidelobes. 

Point Spread Function (PSF)
===
We refer to the PSF derivation of CSAR to deduce the [PSF](/images/rsrch-2019-01-31-4.png) of CASAR, represented with the first-order Bethel Function. The function implies CASAR resolution in cross-track and along-track direction are symmetric and depends on the antenna arrangement. The PSF simulation results of three SAR models in the 2-dimensional array plane is presented below, which shows the high-resolution in cross-track direction and the expected sidelobes suppression of CASAR model.

_PSF simulations results of LASAR, CSAR and CASAR model_

![PSF simulations results of LASAR, CSAR and CASAR model](/images/rsrch-2019-01-31-5.png)

Ground Test Results
===
Our laboratory built a [prototype CASAR system](/images/rsrch-2019-01-31-6.png) and constructed the target scene with [4 homogeneous metal balls of different sizes](/images/rsrch-2019-01-31-7.png). Meanwhile, the Vector Network Analyzer was used to transmit the Step Frequency signal and receive the echo signal. We applied the High Resolution Range Profile technique and 3-dimensional BP imaging algorithm to obtain the 3-dimensional imaging results. Since the CSAR and CASAR both moved in a circular trajectory, we drove the single antenna to move in one circle to form the CSAR model and in a spiral motion to develop the CASAR model. The results prove that CASAR performed well in sidelobes suppression, which is the same as the conclusion we gained in the PSF simulation.

_Ground test results of CSAR and CASAR system_

![Ground test results of CSAR and CASAR system](/images/rsrch-2019-01-31-8.png)