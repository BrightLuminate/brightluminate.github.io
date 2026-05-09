---
layout: single
title: "VFX Compositing Breakdown 01 - Green Screen Keying"
date: 2026-05-09
categories: vfx
tag: [vfx, compositing, after-effects, nuke, green-screen, breakdown]
author_profile: false
---

# VFX Compositing Breakdown 01 - Green Screen Keying

이번 작업은 그린스크린으로 촬영한 인물을 새로운 배경에 자연스럽게 합성하는 연습입니다.  
Keying, Rotoscoping, Tracking, Color Correction 과정을 통해 인물과 배경이 어색하지 않도록 맞추는 것을 목표로 했습니다.

---

## Final Result

아래 영상은 이번 VFX 합성 작업의 최종 결과입니다.
<!-- src="https://www.youtube.com/embed/여기에_유튜브_영상ID" -->

<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden; margin-bottom:30px;">
  <iframe 
    src="https://www.youtube.com/embed/_0lcyyybbng?si=mTtAg_jfGldJxnGD"
    title="VFX Compositing Breakdown 01 - Green Screen Keying"
    style="position:absolute; top:0; left:0; width:100%; height:100%;"
    frameborder="0"
    allowfullscreen>
  </iframe>
</div>

<p align="center">
  <small>Final compositing result video</small>
</p>

---

## Project Overview

이번 프로젝트는 그린스크린으로 촬영한 인물을 배경 영상과 합성하는 작업입니다.  
단순히 배경을 제거하는 것이 아니라, 인물의 가장자리, 색감, 밝기, 그림자, 공간감을 함께 조정하여 자연스러운 합성을 만드는 것에 집중했습니다.

| Category | Description |
| --- | --- |
| 작업 유형 | Green Screen Compositing |
| 사용 프로그램 | After Effects / Nuke |
| 주요 작업 | Keying, Rotoscoping, Tracking, Color Correction |
| 작업 목표 | 인물과 배경의 색감, 조명, 그림자를 자연스럽게 맞추기 |
| 결과물 | Final Composite Video / Before & After / Breakdown |

---

## Before / After

아래 이미지는 원본 영상과 최종 합성 결과를 비교한 이미지입니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/before.jpg" alt="Original Plate" style="width:47%; max-width:100%;">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/after.jpg" alt="Final Composite" style="width:47%; max-width:100%;">
</p>

<p align="center">
  <small>Original Plate / Final Composite</small>
</p>

원본 영상에서는 그린스크린 배경이 남아 있었고, 인물과 배경이 분리되지 않은 상태였습니다.  
최종 결과에서는 배경을 제거한 후 새로운 배경과 인물을 합성하고, 색감과 밝기를 조정하여 자연스럽게 보이도록 작업했습니다.

---

## Breakdown

이번 작업은 아래 순서로 진행했습니다.

---

### 1. Original Plate

먼저 그린스크린으로 촬영된 원본 영상을 확인했습니다.  
인물의 움직임, 조명 방향, 그림자, 그린스크린의 밝기 차이를 확인하며 합성에 필요한 부분을 분석했습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/original-plate.jpg" alt="Original Plate" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Original plate before keying</small>
</p>

---

### 2. Keying

그린스크린 배경을 제거하기 위해 Keying 작업을 진행했습니다.  
인물의 몸통 부분은 비교적 쉽게 분리되었지만, 머리카락과 옷 가장자리 부분은 세밀한 조정이 필요했습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/keying.jpg" alt="Keying Process" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Green screen keying process</small>
</p>

작업 중 집중한 부분은 다음과 같습니다.

- 배경의 초록색 제거
- 인물 가장자리 정리
- 머리카락 주변 디테일 유지
- 초록색 번짐 현상 최소화

---

### 3. Rotoscoping

Keying만으로 깔끔하게 분리되지 않는 부분은 Rotoscoping으로 보정했습니다.  
특히 손, 머리카락, 옷의 외곽선처럼 움직임이 있는 부분을 정리했습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/roto.jpg" alt="Rotoscoping Process" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Rotoscoping and edge cleanup</small>
</p>

Roto 작업은 합성의 완성도를 높이는 중요한 과정이었습니다.  
작은 가장자리 오류도 최종 결과에서는 어색하게 보일 수 있기 때문에 프레임 단위로 확인하며 수정했습니다.

---

### 4. Background Composite

그린스크린을 제거한 인물을 새로운 배경 위에 배치했습니다.  
이 단계에서는 인물의 크기, 위치, 원근감이 배경과 자연스럽게 맞는지 확인했습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/background-composite.jpg" alt="Background Composite" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Character placed on the new background</small>
</p>

---

### 5. Tracking

배경이나 카메라 움직임이 있는 경우, 인물과 배경의 움직임이 따로 놀지 않도록 Tracking을 적용했습니다.  
Tracking을 통해 합성된 인물이 같은 공간 안에 있는 것처럼 보이도록 맞췄습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/tracking.jpg" alt="Tracking Process" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Tracking process for matching movement</small>
</p>

---

### 6. Color Correction

인물과 배경의 색감, 밝기, 대비를 맞추는 Color Correction 작업을 진행했습니다.  
합성에서 가장 중요한 부분 중 하나는 인물과 배경이 같은 조명 환경 안에 있는 것처럼 보이게 만드는 것입니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/color-correction.jpg" alt="Color Correction" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Color correction for matching subject and background</small>
</p>

중점적으로 조정한 부분은 다음과 같습니다.

- 인물의 밝기 조정
- 배경과 색온도 맞추기
- 대비 조정
- 초록색 잔여 색감 제거
- 전체적인 톤 통일

---

### 7. Final Composite

마지막으로 전체 결과를 확인하며 가장자리, 색감, 움직임, 공간감이 자연스러운지 점검했습니다.

<p align="center">
  <img src="{{ site.baseurl }}/assets/images/vfx/green-screen/final-composite.jpg" alt="Final Composite" style="width:850px; max-width:100%;">
</p>

<p align="center">
  <small>Final composite result</small>
</p>

---

## What I Focused On

이번 작업에서 가장 중요하게 생각한 부분은 단순히 배경을 제거하는 것이 아니라,  
인물과 배경이 같은 공간에 있는 것처럼 보이게 만드는 것이었습니다.

특히 아래 부분에 집중했습니다.

- 인물 가장자리의 어색함 줄이기
- 머리카락 주변 디테일 유지
- 배경과 인물의 색감 맞추기
- 조명 방향과 밝기 차이 줄이기
- 최종 영상에서 합성 티가 덜 나도록 조정하기

---

## What I Learned

이번 작업을 통해 Keying만으로는 자연스러운 합성을 만들기 어렵다는 것을 느꼈습니다.  
좋은 합성을 위해서는 Keying 이후에도 Rotoscoping, Edge Cleanup, Color Correction, Tracking 과정이 함께 필요했습니다.

특히 인물과 배경의 색감이 맞지 않으면 아무리 배경 제거가 깔끔해도 합성이 어색해 보일 수 있다는 점을 배웠습니다.

---

## Next Improvement

다음 작업에서는 아래 부분을 더 개선해보고 싶습니다.

- 머리카락 가장자리 디테일 개선
- Light Wrap 적용
- 그림자 추가
- 배경과 인물의 Depth 맞추기
- 더 자연스러운 Color Matching
- Nuke Node 기반 Breakdown 정리

---

## Final Thoughts

이번 Green Screen Keying 작업은 VFX 합성의 기본 과정을 이해하는 데 도움이 되었습니다.  
앞으로는 단순한 배경 제거를 넘어서, 실제 영상 안에 자연스럽게 들어간 것처럼 보이는 합성을 목표로 연습을 이어갈 계획입니다.