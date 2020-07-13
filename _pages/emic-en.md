---
permalink: /emic-en/
layout: splash
title: Elderly Multimodal Interpersonal Conversation
header:
  overlay_color: rgba(23,165,137, 0.5)
  overlay_filter: rgba(255, 0, 0, 0.3)
author_profile: false
last_modified_at: 2020-07-13T14:23:03-05:00
toc: true
---

## Introduction

Elderly Multimodal Interpersonal Conversation Dataset (E-MIC Dataset) is a dataset built to recognize the timing of turn-taking in human-human social interaction. We collected interpersonal conversational interaction data, including video and audio, from 100 elderly people.

![Fig 1_dataset](/assets/emic_dataset.png)[Figure 1] Samples of timing recognition data set for elderly interaction activities

- The subjects are 100 elderly people over the age of 65 (66 women and 34 men, 65~ 85 years old).
- We collected RGB image data with two cameras and audio data with two microphones.
- One session involves two elderly people sitting face to face and interacting with daily conversations, each lasting 15 to 20 minutes.
- The E-MIC dataset includes various conversations (e.g., travel, hobby, health) of the elderly.
- The E-MIC dataset contains conversation interaction data of the elderly from a first-person perspective.
- The E-MIC dataset contains approximately 33 hours of video and three hours of audio data.

## Annotations

We annotated 19 types of information (e.g., take, release, wait, hold, gaze, backchannel, lip state) related to four types of turn-taking.

| **take**   | **hold**     | **release**   | wait            |
| ---------- | ------------ | ------------- | --------------- |
| interrrupt | speech_start | pause         | backchannel     |
| gaze_front | speech_end   | gaze_front    | affirm          |
| lip_open   | gesture_hand | lip_close     | **other_state** |
| negation   |              | **lip_habit** | other_speak     |

The E-MIC dataset used the annotation tool ELAN (https://tla.mpi.nl/tools/tla-tools/elan/download/)) to generate annotations about images and audios.
Annotation information can be edited through the .eaf file included in this dataset and exported (export) in various forms of file (XML, CSV, etc.)

![Fig 2_annotation](/assets/emic_annotation.png)[Figure 2]  Sample of annotation of the collected video and audio clip

## Collected Data

| Collected Data  | File Format   | Size    |
| --------------- | ------------- | ------- |
| RGB videos      | MPEG4         | 89.84GB |
| Audio data      | WAV           | 20.58GB |
| Annotation data | EAF, CSV, XML | 25.24MB |

## Setup Environment

We collected interpersonal conversational interaction data, including video and audio, from 100 elderly people. Figure 3 shows the data collection environment. Participants wear microphones, sit facing each other, and have conversations.

![Fig 3_setup](/assets/emic_setup.png)[Figure 3]  The data collection setup environment: (left) participants wear microphones, sit facing each other, and have conversations.

## Download

Please follow the link below, and join as a member to get to the download page:

- http://nanum.etri.re.kr:8080/etriPortal/login?language=en

## Contact

Please email bettle@etri.re.kr if you have any questions or comments.

## Acknowledgment

- The protocol and consent of data collection were approved by the Institutional Review Board(IRB) at Suwon Science College, our joint research institute.
- This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00162, Development of Human-care Robot Technology for Aging Society].
