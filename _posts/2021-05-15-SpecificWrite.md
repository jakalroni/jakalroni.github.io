---
title: SpecificWrite(특수 문자표 삽입)
tags: etc
key: page-202105150240
summary : GitHub.io 내에서 문자표 삽입, 글머리 기호 등 체험
---

# 0. 소개
 - 앞에 동그라미 문자표
 - 잘 나오나요?

# 1. 개요
``` python
import sys
while True:
    tmp = list(map(int, sys.stdin.readline().split()))
    if tmp[0] == 0:
        break
    max = tmp[0]
    for i in range(tmp[0]):
        for j in range(2, tmp[i + 1] + 1):
            k = 1
            while True:
                try:
                    if j <= tmp[i + k + 1]:
                        k += 1
                    else:
                        break
                except:
                    break
            if k * j > max:
                max = k * j
    print(max)
```

## 1.1. 멕스웰 방정식과 빛의 속도
**목표: 진공상태의 멕스웰 방정식에서 파동방정식을 유도하자.**
$$
\nabla \bullet \vec{E} = \frac{\rho}{\epsilon_0}
$$

---
**3줄 요약**
**1. 진공조건의 멕스웰 방정식을 잘 요리조리(?)하면 파동방정식이 나온다.**
---
즉, 우리는 광속불변의 원리로 파동방정식에서 좌표계의 변환이 특정한 방법으로 이루어져야 함을 알았다.
