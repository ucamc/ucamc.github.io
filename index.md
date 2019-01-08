---
layout: default
---
<section class="hero is-primary">
  <div id="header" class="hero-body">
    <div class="container">
      <h1 class="title is-1">UCAMC</h1>
      <h2 class="subtitle is-4">University of Chicago Applied
      Math Club</h2>
    </div>
  </div>
</section>
<section class="section">
  <div class="container">
    <div id="about-par" class="content">
      <h3 class="title is-3">About us</h3>The <strong>University
      of Chicago Applied Math Club</strong> (UCAMC) is an
      undergraduate club which provides a platform for students
      interested in applications of mathematics and statistics,
      such as in economics (price theory and game theory),
      computer science (complexity theory and data
      science/machine learning), physics and biology. We hold
      meetings where professors and graduate students present on
      their work, and where corporations (e.g. hedge funds and
      cybersecurity firms) discuss the way they use mathematics.
      <br><br>
      <div class="has-text-centered">
      <strong><a href="{{ site.listhost }}">Mailing list</a> | <a href="{{ site.facebookurl }}">Facebook page</a> | <a href="{{ '/suggest' | prepend: site.url }}">Suggest a lecturer</a></strong>
      </div>
    </div>
    <br>
    <h3 id="lectures" class="title is-3">Lectures</h3>
    <h4 class="subtitle is-4">Autumn 2018</h4>
    {% for lecture in site.data.autumn18 %}
    <div class="box">
      <article class="media">
        <div class="media-left">
          <figure class="image is-64x64">
            <a href=
            "{{ lecture.url }}"><img src=
            "{{ lecture.photo | prepend: "/assets/photos/" | prepend: site.url }}"
            alt="Image"></a>
          </figure>
        </div>
        <div class="media-content">
          <div class="content">
            <p><strong>{{ lecture.who }},</strong>
            <i>"{{ lecture.what }}"</i><br>{{ lecture.when }}<br>
            <i>Abstract.</i> {{ lecture.abstract }}</p>
            {% if lecture.youtube %}
            <div class="lecture-link">
              <a href="{{ lecture.youtube }}">Watch the lecture on YouTube</a>
            </div>
            {% endif %}
          </div>
        </div>
      </article>
    </div>
    {% endfor %}
    <br>
    <h3 id="members" class="title is-3">Board members</h3>
    <div id="about-people" class="tile is-ancestor">
      <div class="tile is-parent">
        <article class="tile is-child box">
          <p class="title is-5">Anubhav Nanavaty</p>
          <p class="subtitle is-6">President</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child box">
          <p class="title is-5">Nick Nowicki</p>
          <p class="subtitle is-6">Treasurer</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child box">
          <p class="title is-5">Pol Gómez Riquelme</p>
          <p class="subtitle is-6">Vice President</p>
        </article>
      </div>
      <div class="tile is-parent">
        <article class="tile is-child box">
          <p class="title is-5">Alexander Haberman</p>
          <p class="subtitle is-6">Vice President</p>
        </article>
      </div>
    </div>
  </div>
</section>
