---
permalink: /etri-activity3d-en/
layout: splash
title: ETRI-Activity3D
header:
  overlay_color: rgba(23,165,137, 0.5)
  overlay_filter: rgba(255, 0, 0, 0.3)
author_profile: false
last_modified_at: 2019-11-16T20:23:03-05:00
toc: true
---

A Large-Scale RGB-D Dataset for Robots to Recognize Daily Activity of The Elderly

## Background
&emsp;&emsp; As part of the solutions to an aging society, research on elder care robots has been actively carried out around the world. In order for robots to understand the elderly and provide context-sensitive services, robotic intelligence technologies that can identify various human attributes is essential. Among them, action recognition is a fundamental technology to understand the intentions of human behavior and grasp the daily life patterns of human users. 
<br>&emsp;&emsp;The massive success of the deep learning approach has enabled rapid improvement in many computer vision tasks. Efforts to create large scale datasets to accelerate deep learning studies have been underway in extensive research areas, including human action understanding. However, despite the large number of publicly available datasets, there is a great lack of adequate data for robots to recognize daily activities of human users. Most datasets have no consideration for the robotic environment in which humans and robots live together. Furthermore, there is no large-scale visual dataset at all that deals with the everyday behavior of the elderly. The absence of datasets centered on robots and humans has been a serious impediment to robot intelligence researches, especially for elder care robots.

## Introduction


<figure>
  <img src="/resources/data-samples.png" alt="data-samples"/>
  <figcaption>[Figure 1] Sample frames from daily actions in the proposed dataset are displayed together with the corresponding depth map and skeleton information obtained from Kinect v2 sensors. Actions (from left to right): eating food with a fork, vacuuming the floor, spreading bedding, washing a towel by hands, hanging out laundry, hand shaking.</figcaption>
</figure>

&emsp;&emsp;To solve the shortage of datasets, we collect and release the first large-scale RGB-D dataset of daily activity of the elderly for human care robots: ETRI-Activity3D.
<br>&emsp;&emsp; The dataset is collected by Kinect v2 sensors and consists of three synchronized data modalities: RGB videos, depth maps, and skeleton sequences. To shoot visual data, 50 elderly people are recruited. The elderly subjects are in a wide range of ages from 64 to 88, which lead to a realistic intra-class variation of the actions. In addition, we acquire a dataset for 50 young people in their 20s in the same way as older people. Finally, 112,620 sets of 3D data were obtained.
<br>&emsp;&emsp;We hope that the proposed dataset, which comprehensively considers the elderly, the robots and the environment in which they interact, can contribute to the advancement of robot intelligence.


| Item                    | Contents                                                          |
| :---------------------: | :---------------------------------------------------------------: |
| Number of samples       | 112,620                                                           |
| Number of action classes| 55                                                                |
| Number of subjects      | 100 (50 old people, 50 young people)                              |
| Collection environment  | Residential Environment in Apartment                              |
| Data modalities         | RGB videos, depth map frames, body index frames, 3D skeletal data |
| Sensor                  | Kinect v2                                                         |

Sample videos of our dataset can be downloaded from the link below.

[**Download samples**](https://drive.google.com/open?id=19hgw-kp2qM0rs4-KoaR8Ou8xrjgiQOoD){: target="_blank" }

Unique characteristics and advantages of the proposed dataset over the existing ones are as follows.


**1) A new visual dataset based on observations of the daily activities of the elderly** <br>
**2) A realistic dataset considering the service situation of human care robots** <br>
**3) A large-scale RGB-D action recognition dataset that overcomes the limitations of previous datasets** <br>


## Action Classes

&emsp;&emsp;A closer understanding of what older people actually do in their daily lives is important for determining practical action categories. We visit the homes of 53 elderly people over the age of 70 and carefully monitor and document their daily behavior from morning to night. Based on the most frequent behaviors observed, 55 action classes are defined. 


|  ID | Action descripction                                        | ID |       Action descripction                     | 
| :--:| :---------------------------------------------------------:| :-:| :-------------------------------------------: |
|  1  | eating  food with a fork                                   | 29 |     hanging  out laundry                      |
|  2  |  pouring  water into a cup                                 | 30 |    looking  around for something              |
|  3  |  taking  medicine                                          | 31 |     using a  remote control                   |
|  4  |  drinking  water                                           | 32 |    reading  a book                            |
|  5  |　　putting  food in the fridge/taking food from the fridge 　　  | 33 |     reading  a newspaper                      |
|  6  |  trimming  vegetables                                      | 34 |    handwriting                                |
|  7  |  peeling  fruit                                            | 35 |     talking  on the phone                     |
|  8  |  using a  gas stove                                        | 36 |     playing  with a mobile phone              |
|  9  |  cutting  vegetable on the cutting board                   | 37 |    using a  computer                          |
|  10 | brushing  teeth                                            | 38 |     smoking                                   |
|  11 | washing  hands                                             | 39 |    clapping                                   |
|  12 |  washing  face                                             | 40 |     rubbing  face with hands                  |
|  13 |  wiping  face with a towel                                 | 41 |     doing  freehand exercise                  |
|  14 |  putting  on cosmetics                                     | 42 |    doing  neck roll exercise                  |
|  15 |  putting  on lipstick                                      | 43 |   massaging  a shoulder oneself               |
|  16 |  brushing  hair                                            | 44 |    taking  a bow                              |
|  17 |  blow  drying hair                                         | 45 |    talking  to each other                     |
|  18 |  putting  on a jacket                                      | 46 |    handshaking                                |
|  19 |  taking  off a jacket                                      | 47 |  hugging  each other                          |
|  20 |  putting  on/taking off shoes                              | 48 |   fighting  each other                        |
|  21 | putting  on/taking off glasses                             | 49 |    waving  a hand                             |
|  22 |  washing  the dishes                                       | 50 |　　　　　flapping  a hand up and down (beckoning) 　　　　    |
|  23 |  vacuumming  the floor                                     | 51 |    pointing  with a finger                    |
|  24 |  scrubbing  the floor with a rag                           | 52 | opening  the door and walking in              |
|  25 |  wipping  off the dinning table                            | 53 |    fallen  on the floor                       |
|  26 |  rubbing  up furniture                                     | 54 |    sitting  up/standing up                    |
|  27 |  spreading  bedding/folding bedding                        | 55 |  lying  down                                  |
|  28 |  washing  a towel by hands                                 |    |                                               |

## Collected Data

&emsp;&emsp; The resolution of RGB videos is 1920 × 1080. Depth maps are stored frame by frame in 512 × 424. Skeleton information contains locations of 25 body joints in the 3D space for tracked human bodies.

|  Collected Data   | Resolution | File Format |       Size |
| :---------------: | :--------: | :---------: | ---------: |
|    RGB Videos     | 1920x1080  |     MP4     |     296 GB |
| Depth Map Frames  |  512x424   |     PNG     |     4.08 TB |
| Body Index Frames |  512x424   |     PNG     |    42.60 GB |
| 3D Skeletal Data  | 25 joints  |     CSV     |    20.83 GB |
|                   |            |  **Total**  | **4.44 TB** |

## Setup

&emsp;&emsp; Considering the height of home robots, the shooting device is prepared with two Kinect sensors at heights of 70cm and 120cm as shown in Figure 2. The four shooting devices are grouped together, and eight synchronized sensors in the group capture the subjects' action at the same time. Instead of placing the devices at fixed horizontal angular intervals, we place them in a position where the robot can appear inside the house. The distance between the sensors and the subject also varies from 1.5 meters to 3.5 meters. For actions that can be done anywhere (e.g., taking medicine and talking on the phone), we shoot them up to five times, changing the places where they might occur. In this way, we can provide further intra-class variation by containing different views and background conditions. All the group and camera numbers are provided as the filename for each video sample.

<figure>
  <img src="/resources/data_collection_system_en.png" alt="data_collection_system"/>
  <figcaption>[Figure 2] Configuration of the data acquisition system.</figcaption>
</figure>


## Publications 
<!-- 임시 URL -->
Preprint: [[arXiv]](https://arxiv.org/abs/1810.12541)



## Download
In order to use the dataset, you must be familiar with the EULA(End User License Agreement) and agree to the agreement. Please e-mail the scanned PDF document to the person in charge after you fill out the agreement information. We will provide you with a way to download this dataset if there is no problem with the EULA.

* [Download EULA](/resources/EULA_ETRIActivity3D_en.pdf){: target="_blank" }

## Contact
Please email dhkim008@etri.re.kr if you have any questions or comments.

## Acknowledgment

* The protocol and consent of data collection were approved by the Institutional Review Board(IRB) at Suwon Science College, our joint research institute.
* This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00162, Development of Human-care Robot Technology for Aging Society]. 