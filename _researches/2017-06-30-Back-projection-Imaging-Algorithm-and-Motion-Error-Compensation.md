---
title: "Back-projection Imaging Algorithm and Motion Error Compensation"
collection: researches
permalink: /research/2017-06-30-Back-projection-Imaging-Algorithm-and-Motion-Error-Compensation
excerpt: 'This work designs an autofocus algorithm regarding the image intensity and image contrast to compensate the motion error and realizes the high-quality SAR 2D imaging.'
datestart: 2016-09-30
dateend: 2017-06-01
venue: 'School of Electronic Engineering, UESTC'
program: 'Undergraduate Thesis'
mentor: Prof. Xiaoling Zhang
location: Chengdu, China
---

Back-projection (BP) Imaging Algorithm
===
BP algorithm is a typical time-domain synthetic aperture radar (SAR) imaging method which conducts coherent superposition in the azimuth direction after the range compression. Theoretically, it ignores any approximation, leading to high-quality imaging results. However, the huge computational complexity exists in the value calculation of every pixel one by one in the processing. To improve the execution time, I take advantage of _Matrix Operation_ in MATLAB to use 2D matrix to perform the BP processing instead of reconstructing 2D image point by point. Undergo this change, the time can be cut down by 10%.

* _BP 2D imaging formula_
![BP 2D imaging formula](/images/rsrch-2017-06-30-1.png)

* _BP imaging simulation result_
![BP imaging simulation result](/images/rsrch-2017-06-30-2.png)

Motion Error Compensation
===
The trajectory estimation has a great impact on the focusing of both range direction and azimuth direction in the final 2D SAR image. In practice, the platform movement is not the ideal linear track, but rather irregular which is usually caused by atmospheric turbulence and mechanical vibration made it more difficult to obtain the precise track. The fail in track estimation will create unexpected phase error (or motion error) in the imaging results. Since the accurate distance estimation between the platform and the imaging scene is crucial in high-quality BP SAR imaging, the motion error compensation is required in the BP SAR imaging.

* _phase error occurred in imaging results_
![phase error occurred in imaging results](/images/rsrch-2017-06-30-3.png)

* _BP imaging simulation result with phase error_
![BP imaging simulation result with phase error](/images/rsrch-2017-06-30-4.png)