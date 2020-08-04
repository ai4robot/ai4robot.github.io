---
permalink: /emic/
layout: splash
title: Elderly Multimodal Interpersonal Conversation
header:
  overlay_color: rgba(23,165,137, 0.5)
  overlay_filter: rgba(255, 0, 0, 0.3)
author_profile: false
last_modified_at: 2020-07-13T14:23:03-05:00
toc: true
---

## 소개

고령자 멀티모달 대화 상호작용 데이터셋(Elderly Multimodal Interpersonal Conversation Dataset)은 인간-인간의 사회적 상호작용에서 교류행위(Turn-Taking) 시점을 인식하기 위해 구축한 데이터셋으로, 로봇이 사용자의 대화 시점을 인식해 자연스럽게 상호작용할 수 있는 기술에 적용하기 위한 목적이다. 본 데이터셋은 고령자 100명을 대상으로, 다양한 일상 대화 상호작용을 1인칭 시점으로 수집한 영상과 음성 데이터를 포함한다.

| ![Fig 1_dataset](/assets/emic_dataset.png)  |
| ------------------------------------------- |
| [그림 1] 고령자 대화 상호작용 데이터셋 샘플 |

## 특징

대상자는 고령자 100명(여 66명, 남 34명, 65~85세)이다.
한 세션은 15~20분 분량으로 구성된다.
두명의 고령자가 일상대화(여행, 건강, 운동, 취미 등)를 하는 영상과 음성 데이터를 포함한다.
1인칭 시점의 고령자-고령자 대화 상호작용 데이터를 포함한다.
약 33시간의 영상과 3시간의 음성 데이터를 포함한다.
주석(annotation)은 교류행위 시점과 관련된 19종의 정보를 포함한다.

## 주석(annotation) 정보

주석은 아래와 같이 교류행위 시점 4종(Take: 턴 가져오기, Release: 턴 넘겨주기, Hold: 턴 유지하기, Wait: 맞장구)과 관련된 19종의 정보를 포함한다.

| **take**   | **hold**     | **release**   | wait            |
| ---------- | ------------ | ------------- | --------------- |
| interrrupt | speech_start | pause         | backchannel     |
| gaze_front | speech_end   | gaze_front    | affirm          |
| lip_open   | gesture_hand | lip_close     | **other_state** |
| negation   |              | **lip_habit** | other_speak     |

본 데이터셋은 주석 도구인 ELAN (https://tla.mpi.nl/tools/tla-tools/elan/download/)을 사용해 영상과 음성에 관한 주석을 생성했다.
주석 정보는 본 데이터셋에 포함된 .eaf 파일을 통해 편집이 가능하며, 다양한 형태의 파일 형태(XML, CSV 등)로 내보내기(export) 가능하다.

[그림 2]는 수집한 데이터를 ELAN 도구를 이용해 주석을 생성하는 예를 보여준다.

| ![Fig 2_annotation](/assets/emic_annotation.png)          |
| --------------------------------------------------------- |
| [그림 2] 수집한 대화 상호작용 데이터에  관한 주석 생성 예 |

## 데이터 형식 및 규모

| 수집 데이터     | 데이터 포맷   | 용량    |
| --------------- | ------------- | ------- |
| RGB videos      | MPEG4         | 89.84GB |
| Audio data      | WAV           | 20.58GB |
| Annotation data | EAF, CSV, XML | 25.24MB |

## 수집 환경

본 데이터셋은 일상 주거 환경에서 두 명의 고령자가 마이크를 착용하고 마주보고 대화 상호작용하는 영상과 음성을 수집한다. [그림 3]은 데이터 수집 환경을 보여준다.

| ![Fig 3_setup](/assets/emic_setup.png) |
| -------------------------------------- |
| [그림 3] 데이터 수집 환경              |

## 다운로드

본 데이터셋은 아래 사이트에서 사용허가협약서에 동의하시고 승인을 받으신 후 다운로드 가능합니다.

- **회원 가입 후 다운로드**
  - [링크] http://nanum.etri.re.kr:8080/etriPortal/share/view?id=31

## 담당자 연락처

- 이름: 박천수 책임연구원
- 이메일: bettle@etri.re.kr
- 전화번호: 042-860-1194
- 소속: 한국전자통신연구원 지능로보틱스연구본부 인간로봇상호작용연구실

## 주의

- 본 데이터셋은 개인정보보호와 안전한 데이터의 획득/관리를 위해 기관생명윤리위원회(IRB: Institutional Review Board)의 승인을 거쳐 구축되었습니다.
- 본 데이터셋은 과학기술정보통신부 산하 정보통신기획평가원의“고령 사회에 대응하기 위한 실환경 휴먼케어 로봇 기술 개발(2017-0-00162)”사업의 일환으로 구축되었습니다.