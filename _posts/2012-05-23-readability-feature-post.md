---
layout: post
title: "스크래치 코드 와 파이썬 코드 설명"
date: 2021-07-24
excerpt: "코드설명"
tags: [Scratch, python, 스크래치, 파이썬]
feature: http://i.imgur.com/Ds6S7lJ.png
comments: false
---

---

이번에 설명한 것은 스크래치와 파이썬 입니다 
**스크래치** 에서는 <a href="https://scratch.mit.edu/projects/308755891/" target="_blank">풍차와 전기</a> 를 설명할것이고
파이썬 에서는 **짝수 합산**을 설명을 하겠습니다

---
<iframe id="iframe2" allowtransparency="true" width="700" height="600" frameborder="0" scrolling="no" allowfullscreen="" src="https://jamesbmadden.github.io/scratch-silicon/#308755891"></iframe>

일단 풍차와 전기 부분을 시작하도록 하겠습니다
풍차와 전기에서는 변수와 연산이많이 쓰이고 방송도 쓰입니다

<blockquote class="imgur-embed-pub" lang="en" data-id="a/Mqni0vb"  ><a href="//imgur.com/a/Mqni0vb"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

^ 풍차 날개 코드

풍차 날개 코드를 보시면 일단 변수 2개를 다 0으로 초기화 를 시키고 
**'재시작'** 방송을 보냅니다. 그리고 그 방송을 받으면 ***'전기'*** 라는 변수가
250까지 반복을 합니다 그리고 전기가 250 이다달으면 그즉시회전을 멈추고 전기생산을 멈춥니다

<blockquote class="imgur-embed-pub" lang="en" data-id="a/SBgKaWL" data-context="false" ><a href="//imgur.com/a/SBgKaWL"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

^전구가 켜지는 코드

<blockquote class="imgur-embed-pub" lang="en" data-id="a/jFni9aA" data-context="false" ><a href="//imgur.com/a/jFni9aA"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>

^스위치 코드

일단 시작을했을때에는 전구 코드와 스위치 코드 모양을 기본으로 바꾸고 
버튼 의 변수를 **0과 1로 나눈 뒤** 만약 스위치가 켜져있다면 다음모양으로 바꾸고 전구 방송을 보낸뒤

그리고 전구가 켜지는 코드에서 전구 방송을 받으면 '전기' 라는 변수가 -25가 되고 2초동안 켜지고 꺼지고
off 라는 방송을 보낸다 만약 전기가 20 이하면 모양이 변하지 않고 기존 모양으로 유지된다 
아까 off 라는방송을 보냈는데 off 라는 방송을 받은 전구 코드와 스위치 코드 가 모양이 기본 으로 변한다

---
그다음 파이썬 설명 입니다
짝수 합산부터는 if문이 들어갑니다
짝수 합산을 하기위해 먼저 기본적인 코드 부터 알아야겠죠?

```py
a=0  #a 라는 변수는 0
while a<30: #a 가 30보다 작으면 반복
    a=a+1 #a 가 1씩 증가
    if a%7 is 1:  #만약 a와 7를 나눈값이 1이라면 그다음 실행
        print(a) # a 값 출력
```
if 문만 알고있어도 이번문제인 짝수 합산 문제를 푸실수있습니다

```py 
a=0 #a 라는 변수는 0
b=0 #b 라는 변수는 0
while a<10: #a 가 10보다 작으면 반복
  a=a+1 #a 가 1씩증가
  if a%2 is 0: #만약 a와 2를 나눈값이0이라면 그다음 실행
    b=b+a #b 라는 변수 에다가 위 코드에서 짝수인 숫자를 저장
print(b) #짝수만 더한값을 출력
```
이로써 if 문만 잘신다면 짝수합산이나 홀수합산 등등 여러가지 문제를 푸실수있
