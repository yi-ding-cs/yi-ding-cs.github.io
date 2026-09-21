---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="home-intro">
  <p class="home-lead">I am a <strong>Research Assistant Professor</strong> at the College of Computing and Data Science (CCDS), Nanyang Technological University (NTU), Singapore. I received my Ph.D. in Computer Science and Engineering from NTU under the supervision of <a href="https://ntu-cbcr.org/" target="_blank">Prof. Cuntai Guan</a>.</p>

  <p>My research vision is to build <strong>brain-aware artificial intelligence</strong> that can understand, generalize, and ultimately augment human affective and cognitive states. I work at the intersection of <strong>brain-computer interfaces (BCIs), neural signal decoding, affective computing, and deep learning</strong>, with a particular focus on EEG.</p>

  <p>A distinctive thread across my work is the integration of <strong>neurophysiological and neuropsychological knowledge</strong> into modern learning systems. I design models around how brain activity is organized across regions, time, and cognitive processes. I combine this model-design perspective with <strong>cross-subject and cross-task generalization</strong>, foundation-model learning, and translation toward real-world mental-health and human-computer-interaction applications.</p>

  <p>My long-term goal is to connect <strong>brain science, generalizable AI, and clinical translation</strong>: developing models that are scientifically grounded, scalable across people and tasks, and useful beyond the laboratory.</p>
</div>

## Research

<div class="research-pillars">
  <div class="research-pillar">
    <div class="pillar-icon"><i class="fas fa-brain" aria-hidden="true"></i></div>
    <h3>Neurophysiology-inspired AI</h3>
    <p>Neural architectures that encode brain organization, functional connectivity, temporal dynamics, and cognitive priors rather than relying only on generic deep-learning structures.</p>
  </div>

  <div class="research-pillar">
    <div class="pillar-icon"><i class="fas fa-wave-square" aria-hidden="true"></i></div>
    <h3>Generalizable EEG Intelligence</h3>
    <p>Cross-subject, cross-dataset, and cross-task neural decoding, including EEG foundation models and transferable representations for affective and cognitive states.</p>
  </div>

  <div class="research-pillar">
    <div class="pillar-icon"><i class="fas fa-heart-pulse" aria-hidden="true"></i></div>
    <h3>Translational Brain-Computer Interfaces</h3>
    <p>Multimodal and clinically oriented BCI systems for emotion understanding, mental health, cognitive-state modeling, neurofeedback, and human-computer interaction.</p>
  </div>
</div>

<div class="research-keywords">
  <span>Brain-Computer Interfaces</span>
  <span>Affective Computing</span>
  <span>EEG Foundation Models</span>
  <span>Neural Signal Decoding</span>
  <span>Multimodal Learning</span>
  <span>AI for Mental Health</span>
</div>

## News

<div class="news-scroll" aria-label="Latest news">
{% for item in site.data.news %}
  <div class="news-item">
    <div class="news-date">{{ item.date }}</div>
    <div class="news-text">{{ item.text }}</div>
  </div>
{% endfor %}
</div>
<p class="section-note">Scroll to see earlier updates.</p>

## Selected Publications

<div class="selected-papers">
{% for paper in site.data.selected_papers %}
  <article class="paper-card">
    <div class="paper-thumb">
      <img src="{{ paper.image | relative_url }}" alt="Visual summary for {{ paper.title }}" loading="lazy">
    </div>
    <div class="paper-content">
      <h3>
        {{ paper.title }}
        {% if paper.highly_cited %}<span class="highly-cited" title="Highly Cited Paper"><i class="fas fa-trophy" aria-hidden="true"></i></span>{% endif %}
      </h3>
      <p class="paper-authors">{{ paper.authors }}</p>
      <p class="paper-venue"><strong>{{ paper.venue }}</strong>{% if paper.highly_cited %} · <span class="highly-cited-label">Highly Cited</span>{% endif %}</p>
      <p class="paper-summary">{{ paper.summary }}</p>
      <div class="paper-links">
        <a class="paper-link" href="{{ paper.paper }}" target="_blank" rel="noopener"><i class="fas fa-file-pdf" aria-hidden="true"></i> Paper</a>
        {% if paper.code %}<a class="paper-link" href="{{ paper.code }}" target="_blank" rel="noopener"><i class="fab fa-github" aria-hidden="true"></i> Code</a>{% endif %}
      </div>
    </div>
  </article>
{% endfor %}
</div>

<p class="all-publications-link"><a href="{{ '/publications/' | relative_url }}"><strong>View more publications →</strong></a></p>

## Academic Profile

I have authored or co-authored **30+ peer-reviewed papers** in venues including *IEEE TPAMI, IEEE TNNLS, IEEE TIP, IEEE TAFFC, IEEE J-BHI, IEEE Signal Processing Magazine, ICLR, ICML, NeurIPS, AAAI,* and *ACM Multimedia*. My work spans foundational EEG representation learning, affective BCIs, multimodal emotion modeling, and translation of neural-decoding methods toward healthcare applications.

<p>
  <a href="{{ '/cv/' | relative_url }}" class="all-publications-link">
  <strong>  View Detailed Academic Profile →</strong>
  </a>
</p>

For research collaboration, student supervision, or academic enquiries, please contact me at [ding.yi@ntu.edu.sg](mailto:dingyi.scse@gmail.com).
