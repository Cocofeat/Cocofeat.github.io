---
layout: academic
permalink: /
description: Coco Ke Zou is a Research Fellow at the National University of Singapore studying uncertainty, external validation, and grounded reasoning in medical AI.
redirect_from:
  - /about/
  - /about.html
---
{% assign profile = site.data.profile %}
<div class="wrap home">
  <div class="home-intro" id="about-me">
    <header class="home-identity">
      <h1>{{ profile.name }} <span lang="zh">{{ profile.native_name }}</span></h1>
      <p class="home-affiliation">
        {{ profile.role }} ·
        <a href="{{ site.author.nusdiscovery }}">
          <svg aria-hidden="true" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" style="vertical-align:-.15em">
            <path d="M3 9 12 4l9 5H3Zm2 2v7m5-7v7m4-7v7m5-7v7M3 20h18"/>
          </svg>&nbsp;{{ profile.affiliation }}
        </a>
      </p>
      <p class="home-links">
        <a href="{{ '/cv/' | relative_url }}">
          <svg aria-hidden="true" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" style="vertical-align:-.15em">
            <path d="M6 3h8l4 4v14H6zM14 3v5h4M9 12h6m-6 4h6"/>
          </svg>&nbsp;CV
        </a>
        <a href="{{ site.author.googlescholar | escape }}">
          <svg aria-hidden="true" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" style="vertical-align:-.15em">
            <path d="m2 9 10-4 10 4-10 4zM6 11v5c3 3 9 3 12 0v-5m4-2v6"/>
          </svg>&nbsp;Google Scholar
        </a>
        <a href="https://github.com/{{ site.author.github }}">
          <svg aria-hidden="true" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" style="vertical-align:-.15em">
            <path d="m8 7-5 5 5 5m8-10 5 5-5 5M14 5l-4 14"/>
          </svg>&nbsp;GitHub
        </a>
        <a href="mailto:{{ profile.email }}">
          <svg aria-hidden="true" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" style="vertical-align:-.15em">
            <rect x="3" y="5" width="18" height="14" rx="2"/>
            <path d="m4 7 8 6 8-6"/>
          </svg>&nbsp;Email
        </a>
      </p>
    </header>
    <img class="home-portrait" src="{{ '/images/ke-zou-450.webp' | relative_url }}" width="450" height="600" fetchpriority="high" alt="Portrait of {{ profile.name }}">
  </div>

  <section class="home-section home-biography" id="research">
    <h2>Biography and research</h2>
    <div id="-educations">{{ profile.bio | markdownify }}</div>
    <p id="roadmap"><strong>I study how medical AI can recognize uncertainty, ground its decisions in clinical evidence, and generalize across populations.</strong> I focus on three questions:</p>
    <ul class="home-research">
      <li id="trustworthy-medical-image-analysis"><a href="{{ '/research/#trustworthy' | relative_url }}"><strong>When should a model defer?</strong></a> I develop <strong>uncertainty estimation</strong> and calibration methods for medical image analysis.</li>
      <li id="explainable-and-groundable-vlm"><a href="{{ '/research/#explainable' | relative_url }}"><strong>Can clinicians verify a model’s reasoning?</strong></a> I connect diagnostic language to image evidence and study how <strong id="agentsagentic-for-specialists">VLMs or AI agents</strong> can verify evidence and escalate uncertain cases.</li>
      <li id="fm-for-generalists"><a href="{{ '/research/#foundation' | relative_url }}"><strong>Does performance transfer across populations?</strong></a> I benchmark <strong>medical foundation models</strong> on external cohorts and study how much labeled data they need.</li>
    </ul>
  </section>

  <section class="home-section" id="-publications">
    <span id="-selected-publications--means-co-first-author"></span>
    <div id="-experiences">
      <div class="home-section-heading">
        <h2>Featured work</h2>
        <a href="{{ site.author.googlescholar | escape }}" aria-label="All publications on Google Scholar">All publications</a>
      </div>
      {% include featured-projects.html compact=true %}
    </div>
  </section>

  <section class="home-section" id="-news">
    <h2>Recent news</h2>
    {% assign recent_news = site.data.news | slice: 0, 5 %}
    {% assign archive = site.data.news | slice: 5, site.data.news.size %}
    {% include news-items.html items=recent_news %}
    <details class="archive">
      <summary>Earlier updates ({{ archive.size }})</summary>
      {% include news-items.html items=archive %}
    </details>
  </section>

  <section class="home-section" id="-activities">
    <span id="guest-editors"></span><span id="handling-editor"></span><span id="area-chairs"></span><span id="reviewers"></span>
    <h2>Academic activities</h2>
    <ul class="home-activity-list">
      {% for appointment in site.data.record.editorial_appointments %}
        <li><strong>{{ appointment.role | escape }}</strong> · {{ appointment.venue | escape }}</li>
      {% endfor %}
      {% for appointment in site.data.record.conference_appointments %}
        <li><strong>{{ appointment.role | escape }}</strong> · {{ appointment.venue | escape }}</li>
      {% endfor %}
      <li><a href="{{ '/service/#peer-review' | relative_url }}">Journal and conference peer review</a></li>
      <li><a href="{{ '/cv/#projects' | relative_url }}">Research funding</a></li>
      <li id="-academic-visits-and-exchanges"><a href="{{ '/cv/#exchanges' | relative_url }}">Academic visits and exchanges</a></li>
      <li id="-talks"><a id="-talks-and-presentations" href="{{ '/teaching/#talks' | relative_url }}">Talks and presentations</a></li>
    </ul>
  </section>

  <section class="home-section" id="-honors-and-awards">
    <h2>Honors and awards</h2>
    <ul class="home-activity-list">
      <li><strong>NUS Medicine Outstanding Research Fellow Award</strong> · First runner-up, 2026</li>
      <li><strong>Best Poster Award</strong> · 13th Medical Imaging Computing Seminar (MICS), 2026</li>
    </ul>
    <p><a href="{{ '/cv/#honors' | relative_url }}">All honors and awards</a></p>
  </section>

  <section class="home-section split" id="contact">
    <div>
      <h2>Contact</h2>
      <p>I welcome collaborations on uncertainty estimation, multimodal medical foundation models, and trustworthy agentic AI for healthcare.</p>
      <p class="home-links">
        <a href="{{ site.author.nusdiscovery }}">NUS Discovery</a>
        <a href="{{ site.author.orcid }}">ORCID</a>
        <a href="{{ site.author.pubmed }}">PubMed</a>
        <a href="https://www.linkedin.com/in/{{ site.author.linkedin | uri_escape }}">LinkedIn</a>
      </p>
    </div>
    <figure>
      <a href="https://s01.flagcounter.com/more/V8">
        <img src="https://s01.flagcounter.com/map/V8/size_s/txt_000000/border_CCCCCC/pageviews_0/viewers_0/flags_0/"
             alt="Visitor map of the homepage" width="400" height="205"
             loading="lazy" style="display:block;max-width:100%;height:auto">
      </a>
    </figure>
  </section>
</div>
