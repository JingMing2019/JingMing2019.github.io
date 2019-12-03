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

![BP 2D imaging formula](/images/rsrch-2017-06-30-1.png){: .align-center}

* [_BP imaging simulation result_](/images/rsrch-2017-06-30-2.png)

Motion Error Compensation
===
The trajectory estimation has a great impact on the focusing of both range direction and azimuth direction in the final 2D SAR image. In practice, the platform movement is not the ideal linear track, but rather irregular which is usually caused by atmospheric turbulence and mechanical vibration made it more difficult to obtain the precise track. The fail in track estimation will create unexpected phase error (or motion error) in the imaging results. Since the accurate distance estimation between the platform and the imaging scene is crucial in high-quality BP SAR imaging, the motion error compensation is required in the BP SAR imaging.

* _phase error occurred in imaging results_

![phase error occurred in imaging results](/images/rsrch-2017-06-30-3.png){: .align-center}

* [_BP imaging simulation result with phase error_](/images/rsrch-2017-06-30-4.png)

Autofocus Algorithm
===
Autofocus algorithm compensates the motion error based on the radar echo signals which works on the signal processing layer, rather than make any effort to acquire the high-accurate trajectory data with high-quality motion sensors. At first, the existing autofocus algorithm based on maximum image intensity is simulated, and the imaging result is not as much as expected.

* _imaging results of existing autofocus algorithm based on maximum image intensity_

![imaging results of autofocus algorithm based on based on maximum image intensity](/images/rsrch-2017-06-30-5.png){: .align-center}

To improve the imaging results, the thesis proposes an **autofocus algorithm based on maximum image contrast** to figure out the phase error for BP SAR imaging. The theory behind is the positive relationship between the SAR images focusing level and its image contrast. The problem of focusing can be converted to the [determination of maximum contrast.](/images/rsrch-2017-06-30-6.png)

* _phase error compensation of autofocus algorithm based on maximum image contrast_

![phase error compensation of autofocus algorithm based on maximum image contrast](/images/rsrch-2017-06-30-7.png){: .align-center}

To acquire the high-quality focusing SAR 2D imaging results, the work combines the two autofocus algorithm which applies image intensity to estimate the proper antenna phase centre and introduces image contrast to improve the image quality.

* _imaging results of combined autofocus algorithm_

![imaging results of autofocus algorithm based on maximum image contrast](/images/rsrch-2017-06-30-8.png){: .align-center}