---
layout: post
title:  "Converting Moniwiki to Jekyll"
date:   2015-07-04 12:00:00
categories: blog jekyll
---
Jekyll 로 블로그를 만들어보려고 하는데 기존에 사용하던 Moniwiki 페이지가 버리기엔 아깝고 둘다 쓰기에는 벅참
Moniwiki를 Jekyll 로 변환해보기로 함

# Plan
 * 한글제목의 페이지 때문에 생긴 아스키코드 형태의 링크들의 리스트 추출. 한글 원제목도 함께 추출
 * 크롤러를 구현해서 기존 Moniwiki의 모든 HTML의 페이지를 저장 ( script, css 제외. only HTML )
 * 파일명과 링크를 가시적인 영문으로 변경할 방법 모색
 * 모든 HTML 문서를 Makrdown 문서로 변환
 * 모든 Markdown 문서에 Jekyll header 추가
 * Moniwiki 페이지들의 링크구조를 Blog 형태에 맞게 재구성

# Execute

### References
 * [HTML2Markdown](https://github.com/aaronsw/html2text)