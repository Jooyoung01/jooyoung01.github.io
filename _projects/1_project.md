---
layout: page
title: Truck Detection and Counting
description: Study on Truck Detection and Counting Using Infrared Cameras
img: assets/img/proj_pic/truck_detection.png
importance: 1
category: Research1
---

    title: Truck Detection and Counting in Low-Light Condition: Do We Need Infrared Camera?
    description: Research on the Necessity of Infrared Cameras for 24-Hour CCTV Truck Detection: Identifying and Accurately Counting Trucks Impacting Environmental Pollution.
    tool: YOLO, Pytorch, OpenCV


These are video samples of a deep learning model trained on Regular and Infrared data for truck detection.

<div class="row justify-content-sm-center">
  <div class="col-sm mt-3 mt-md-0">
    {% include video.liquid loading="eager" path="assets/video/truck_detection.mp4" title="Truck video" class="img-fluid z-depth-1" controls=true autoplay=true %}
  </div>
</div>
<div class="caption">
The videos on the left column were captured by a regular camera, while the videos on the right column were taken using an infrared camera. The top row of videos were taken during the daytime, while the bottom row features nighttime footage. 
</div>
The models were trained on separate datasets. Both the regular and infrared cameras were synchronized during the recording process. The video datasets were recorded by me and my team on the California 710 freeway, a location well-known for its heavy truck traffic.
<div class="row justify-content-sm-center">
  <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/proj_pic/truck_resutls.png" title="truck result image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

Table 3 demonstrates that the model trained on nighttime Infrared Video (F1-score 0.903) outperforms the model trained on nighttime Regular Video (F1-score 0.804). Moreover, Table 4 shows that the detection rate of trucks in the right lane during nighttime using Regular video is relatively poor.
<br/>

Abstract: <br/>
Conventional visual traffic analysis methods face challenges in achieving accurate and cost-effective monitoring of truck movements, especially in adverse conditions (bad weather or nighttime). The advent of deep learning technology has revolutionized object detection such as vehicles, particularly using low-cost Closed-Circuit Television (CCTV) cameras. However, object detection in low-light conditions such as nighttime is still a challenge. To address these challenges, we explore the potential of infrared imaging compared to regular imaging in truck detection and counting. Our study compares the performance of a YOLO- v5s model trained under various conditions for truck detection and counting, including day and night settings with temporally synchronized Regular and Infrared (IR) videos collected at the California 710 Freeway. Our experimental results confirmed that utilizing IR videos provides a better detection accuracy at night as expected. However, we found that just using regular videos in a specific way such as monitoring trucks at a closer distance in urban streets generates a satisfactory result which is comparable to that of IR videos. This is because there are still some lights around urban freeways even at night and hence, a regular camera is still able to successfully capture the edges of trucks. Furthermore, when the goal of monitoring truck movements is to count the number of passing trucks in a video, the accuracy of truck detection in an image is less critical than the performance of a counting algorithm.
<br/>

- J. Yoo, S. H. Kim, K. Sukhani, M. S. Yoo and C. Shahabi, "Truck Detection and Counting in Low-Light Condition: Do We Need Infrared Camera?," 2024 IEEE International Conference on Big Data and Smart Computing (BigComp), Bangkok, Thailand, 2024, pp. 317-324, [doi: 10.1109/BigComp60711.2024.00057](https://doi.org/10.1109/BigComp60711.2024.00057)
.
