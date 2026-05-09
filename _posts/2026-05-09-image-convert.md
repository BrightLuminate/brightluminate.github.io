---
layout: single
title: "NumPy로 이미지 파일 변환하기"
date: 2026-05-09
categories: coding
tag: [python, blog, jekyll, github]
author_profile: false
redirect_from:
# sidebar:
#     nav: "counts" 
---




**[공지사항]** [지킬 블로그 공식 문서](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
{: .notice--warning}

# NumPy로 이미지 파일 변환하기

파이썬에서 이미지 파일을 NumPy 배열로 변환하는 방법을 알아보겠습니다.

<p style="text-align:right;">
NumPy와 PIL을 사용하여 이미지를 배열 형태로 변환합니다.
</p>

[구글 바로가기](https://google.com){: .btn .btn--info}

## 전체 코드

```python
import numpy as np
import matplotlib.pyplot as plt
from PIL import Image
import os

# 이미지 디렉토리 경로
image_path = '/Users/choedohyeon/Downloads/data/cloudy'

# 디렉토리 내 파일 리스트 가져오기
img_list = os.listdir(image_path)

# jpg 파일만 필터링
img_list_jpg = [img for img in img_list if img.endswith(".jpg")]

print("img_list_jpg:", img_list_jpg)

# NumPy 배열 저장 리스트
img_list_np = []

# 이미지 반복 처리
for img_name in img_list_jpg:

    img_path = os.path.join(image_path, img_name)

    print("열기를 시도 중:", img_path)

    try:
        # 이미지 열기
        img = Image.open(img_path)

        # NumPy 배열 변환
        img_array = np.array(img)

        # 리스트 저장
        img_list_np.append(img_array)

        print(img_name, "이미지 shape :", img_array.shape)

    except FileNotFoundError:
        print(f"파일을 찾을 수 없습니다: {img_path}")

# 리스트 → NumPy 배열 변환
img_np = np.array(img_list_np)

print("img_np shape:", img_np.shape)

# 마지막 이미지 출력
if len(img_list_np) > 0:

    plt.imshow(img_list_np[-1])

    plt.title("Last Image")

    plt.axis("off")

    plt.show()

else:
    print("불러온 이미지가 없습니다.")
```

## 실행 결과

![zps]({{ site.baseurl }}/assets/images/2024-05-01-e/zps.png)

---

# 코드 설명

## 1. 라이브러리 불러오기

- `numpy`
- `matplotlib`
- `PIL`
- `os`

이미지 처리 및 시각화를 위해 사용합니다.

---

## 2. 이미지 경로 설정

```python
image_path = '/Users/choedohyeon/Downloads/data/cloudy'
```

이미지가 저장된 폴더 경로입니다.

---

## 3. jpg 파일만 추출

```python
img_list_jpg = [img for img in img_list if img.endswith(".jpg")]
```

`.jpg` 확장자 파일만 가져옵니다.

---

## 4. 이미지 NumPy 배열 변환

```python
img_array = np.array(img)
```

이미지를 배열 형태로 변환합니다.

---

## 5. 마지막 이미지 출력

```python
plt.imshow(img_list_np[-1])
```

마지막으로 불러온 이미지를 화면에 출력합니다.