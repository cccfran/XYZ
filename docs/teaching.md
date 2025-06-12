---
layout: default
title: Teaching
nav_order: 4
---

# Teaching
{: .no_toc }

## Urban Analytics (ITAO 40570 / MSBR 70580)

### ML in Urban Analysis

Spring 2023, 2024 (Elective for <a href='https://realestate.nd.edu/education/undergraduate-minor/curriculum/'>Real Estate Minor</a>)

<a href="https://jh-cai.com/docs/Syllabus_ITAO40570.pdf">Syllabus</a>

<div class="row" id="myItems">
  <div class="col-sm-12 mb-3">
    <!-- <span id="{{ type | join: '_' }}"></span>
    <h2 style="display:inline;"> {{ type }}s </h2> -->
    <!-- <h5 style="text-align:right;float:right;"><a href="#top">[ Top ]</a></h5>  -->
    {% assign topics = site.data.urban_analytics | sort: 'id' %}
    {% for utopic in topics %}
    {% assign counter = counter | plus: 1 %}
    <div class="card border-light">
      <div class="card-body">
        <h3 class="card-title"><a data-toggle="collapse" data-target="#collapseAbstractu{{ utopic.id }}" aria-expanded="false" aria-controls="collapseAbstractu{{ utopic.id }}" href="">{{ utopic.id }}. {{ utopic.title }}</a></h3>
        <h4 class="card-subtitle">{{ utopic.case }}</h4>
        <h5 class="card-text"> 
          <p> {{ paper.desc }} </p>
        </h5>
        <div class="collapse" id="collapseAbstractu{{ utopic.id }}">
          <div  class="row">
          <div class="col-9">
            <h5 class="card-text"> 
              <div class="container" style="text-align:justify">
            <!-- <hr/> -->
                <p style="font-size:15px">
                {{ utopic.desc }}
                </p>
                {% if utopic.url %}
                <a href="{{ utopic.url }}">Google Drive</a>
                {% endif %}
              </div>
            </h5>
          </div>
          <div class="col-3">
            <img src="{{ utopic.pic }}" alt="">
          </div>
        </div>
        </div>
        <!-- <div class="collapse" id="collapseDescription{{ paper.id }}">
          <div class="container">
            <hr/>
            {{ paper.description }}
          </div>
        </div> -->
      </div>
    </div>  
    {% endfor %}
  </div>
</div>


## Modern Data Mining

<div class="card border-light">
<div class="card-body"> 
  <h3 class="card-title">
  </h3>
  <h5 class="card-subtitle text-muted pb-2">   
  </h5>
      <h5 class="card-text"> 
        <div class="container" style="text-align:justify">
          <p style="font-size:18px">
            This is a cross-listed course with a student body mixed with advanced undergraduates, masters, MBAs, and Ph.D.s.
The course covers data science essentials -- a wide selection of supervised and unsupervised learning methods and keeps pace with state-of-the-art methods.
It focuses on the statistical ideas and machine learning methodologies that will equip students to analyze modern complex and large-scale data. 
          <ul style="font-size:18px">
            <li>Co-developed STAT 471/571/701 Modern Data Mining (head TA Spring 2021 and TA Fall 2017)</li>
            <li>Wharton Executive Education OneConnect Program with Two Sigma (Summer 2019)</li>
            <li>Wharton Data Science Academy of Wharton Youth Program (Summer 2021)</li>
            <li>Data Science Live: <a href="https://jh-cai.com/dsl2019/"> DSL1 </a><a href="https://jh-cai.com/dsl2019fall/"> DSL2 </a><a href="https://jh-cai.com/modern-data-mining/dsl.html"> DSL3 </a><a href="https://jh-cai.com/modern-data-mining/dsl4.html">DSL4</a></li>
            <li><a href="https://jh-cai.com/docs/syllabus_STAT471571701.pdf">Syllabus</a></li>
          </ul>
          </p>
        </div>  
      </h5>
</div>
</div>


<div class="row" id="myItems">
  <div class="col-sm-12 mb-3">
    <!-- <span id="{{ type | join: '_' }}"></span>
    <h2 style="display:inline;"> {{ type }}s </h2> -->
    <!-- <h5 style="text-align:right;float:right;"><a href="#top">[ Top ]</a></h5>  -->
    {% assign topics = site.data.modern-data-mining | sort: 'id' %}
    {% for topic in topics %}
    {% assign counter = counter | plus: 1 %}
    <div class="card border-light">
      <div class="card-body">
        <h3 class="card-title"><a data-toggle="collapse" data-target="#collapseAbstract{{ topic.id }}" aria-expanded="false" aria-controls="collapseAbstract{{ topic.id }}" href="">{{ topic.id }}. {{ topic.title }}</a></h3>
        <h5 class="card-text"> 
          {{ paper.desc }}
        </h5>
        <div class="collapse" id="collapseAbstract{{ topic.id }}">
          <div  class="row">
          <div class="col-9">
            <h5 class="card-text"> 
              <div class="container" style="text-align:justify">
            <!-- <hr/> -->
                <p style="font-size:15px">
                {{ topic.desc }}
                </p>
              </div>
            </h5>
          </div>
          <div class="col-3">
            <img src="{{ topic.pic }}" alt="">
          </div>
        </div>
        </div>
        <!-- <div class="collapse" id="collapseDescription{{ paper.id }}">
          <div class="container">
            <hr/>
            {{ paper.description }}
          </div>
        </div> -->
      </div>
    </div>  
    {% endfor %}
  </div>
</div>

<!-- 
{% assign courses = site.data.teaching | where:"type","instructor" %}
{% for course in courses %}
{% assign course = course_hash[1] %}
<div class="card border-light">
<div class="card-body"> 
  <h3 class="card-title">{{ course.title }}</h3>
  <h5 class="card-subtitle text-muted pb-2"> 
  {% for time in course.time %}
    {% if forloop.index < course.time.size %} 
    {{ time.time }},
    {% else %} {{ time.time }}
    {% endif %}
  {% endfor %}
  </h5>
  <h5 class="card-text"> 
  </h5>
</div>
</div>

{% endfor %} -->

<!-- <br>  -->

<!-- ## TA
{: .no_toc }

{% assign courses = site.data.teaching | where:"type","TA" %}
{% for course in courses %}
{% assign course = course_hash[1] %}
<div class="card border-light">
<div class="card-body"> 
  <h3 class="card-title">{{ course.title }}</h3>
  <h5 class="card-subtitle text-muted pb-2"> 
  {% for time in course.time %}
    {% if forloop.index < course.time.size %} 
    {{ time.time }},
    {% else %} {{ time.time }}
    {% endif %}
  {% endfor %}
  </h5>
  {% if course.more %}
  <h5 class="card-text"> 
  	<a href="{{ course.more }}">Data Science Live (DSL)</a>
  </h5>
  {% endif %}
</div>
</div>
{% endfor %} -->