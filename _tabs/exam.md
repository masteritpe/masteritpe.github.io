---
layout: page
icon: fas fa-graduation-cap
order: 2
title: 출제예상
---

> 정보관리기술사 회차별 출제 예상 토픽 시리즈. 기출 + 모의/합숙 + 최근 뉴스 트렌드를 분석해 회차별 핵심 토픽을 선정합니다.
{: .prompt-info }

<!-- [출제예상 포스트 필터링 가이드] 
     'exam-prediction' 태그가 달린 포스트들을 최신순으로 정렬하여 표시합니다. -->
{% assign exam_posts = site.posts | where_exp: "post", "post.tags contains 'exam-prediction'" | sort: 'date' | reverse %}

{% if exam_posts.size == 0 %}
포스트 준비 중입니다.
{% else %}

## 출제 대비 토픽 리스트

{% for post in exam_posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — `{{ post.categories | first }}`
{% endfor %}

{% endif %}

---

- 기출 데이터: [KPC 정보관리기술사 기출·합숙·모의 통합 검색](https://kpcitpe-search.pages.dev/){:target="_blank"}

> 예측은 학습 참고용이며 출제를 보장하지 않습니다.
{: .prompt-warning }
