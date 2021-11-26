---
permalink: /etri-activity3d-livinglab-en/
layout: splash
title: ETRI-Activity3D-LivingLab
header:
  overlay_color: rgba(23,165,137, 0.5)
  overlay_filter: rgba(255, 0, 0, 0.3)
author_profile: false
last_modified_at: 2021-03-17T17:30:03-05:00
toc: true
---

# A RGB-D Activity Dataset Built in Actual Residential Spaces of The Elderly

## Introduction

<figure>
  <img src="/assets/livinglab-data-samples.png" alt="data-samples"/>
  <figcaption>[Figure 1] Sample frames of ETRI-Activity3D-LivingLab dataset. Samples are displayed with the corresponding depth map and skeleton data. Activities(from left to right): taking medicine, taking off a jacket, vacuuming the floor, using a remote control.</figcaption>
</figure>

&emsp;&emsp;We introduce ETRI-Activity3D-LivingLab, realistic dataset for more practical activity recognition studies in robot environments. The dataset was built in a residential environment where the elderly actually live, not in a testbed. We visited 50 households where elderly people live alone and acquired 8,622 3D visual data from the robot’s point of view. 

&emsp;&emsp;Our dataset aims to reflect as much as possible the situation that robots serve. We constructed a capturing equipment with Kinect v2 sensors installed at 70cm and 120cm heights considering the height of the home service robots. The equipment was placed in various locations where robots may exist in the home. The distance between the camera and the target human varies from 1.5 m to 3.5 m.

&emsp;&emsp;ETRI-Activity3D-LivingLab is meaningful in that it is the first 3D activity recognition dataset acquired from the robot perspective in various residential spaces where the elderly live.


| Item                    | Contents                                                          |
| :---------------------: | :---------------------------------------------------------------: |
| Number of samples       | 8,622                                                             |
| Number of action classes| 55                                                                |
| Number of subjects      | 50 (8 males, 42 females)                                          |
| Collection environment  | The actual home environments of the elderly living alone          |
| Obtaining location      | Various places that robots can be located                         |
| Data modalities         | RGB videos, depth map frames, body index frames, 3D skeletal data |
| Sensor                  | Kinect v2                                                         |

Sample videos of our dataset can be downloaded from the link below.

* [ETRI-Activity3D-Living_Samples](https://drive.google.com/open?id=19hgw-kp2qM0rs4-KoaR8Ou8xrjgiQOoD){: target="_blank" }

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

|  Collected Data   | Resolution | File Format |         Size |
| :---------------: | :--------: | :---------: | -----------: |
|    RGB Videos     | 1920x1080  |     MP4     |       42.4GB |
| Depth Map Frames  |  512x424   |     PNG     |     512.20GB |
| Body Index Frames |  512x424   |     PNG     |       7.04GB |
| 3D Skeletal Data  | 25 joints  |     CSV     |       5.49GB |
|                   |            |  **Total**  | **567.13GB** |

## Download
Please follow the link below, and join as a member to get to the download page:
* [ETRI-AI-NANUM](https://nanum.etri.re.kr/share/list?lang=En_us)

## Contact
Please email [dhkim008@etri.re.kr](mailto:dhkim008@etri.re.kr) if you have any questions or comments.

## Acknowledgment

* The protocol and consent of data collection were approved by the Institutional Review Board(IRB) at Suwon Science College, our joint research institute.
* This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00162, Development of Human-care Robot Technology for Aging Society].