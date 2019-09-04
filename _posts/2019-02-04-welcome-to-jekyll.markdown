---
layout: post
title:  "탐사 기획보도"
categories: [ Jekyll ]
image: assets/images/demo1.jpg
---
분석 가능 범위는 취재 방향을 구체화하기 위한 기자님이 원하시는 특정 이슈지역분석,각 도시별 시계열 가격변동률 확인 및 비교분석,신도시 vs 비신도시, 신도시 vs 서울 비교분석
2기 신도시 이후 가격변동률 큰 지역과 작은 지역 발굴, 3기 신도시 발표 후 해당지역 및 인근지역의 가격변동 확인, 매매값 vs 전세값 비교.

분석 과정은 수도권 약 18,230개의 아파트를 대상으로 약390만건의 아파트실거래매매가격 데이터를 다운로드한다. 다운로드한 데이터는 DB로 업로딩하여 주소정제 및 데이터 클렌징을 통한 분석가능 데이터 형태로 변경한다. 그 뒤 빅데이터분석 및 GIS분석을 진행한다.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
