---
layout: default
title: Home
permalink: /
---

<section class="profile">
  <img class="profile-photo" src="{{ '/assets/images/profile.png' | relative_url }}" alt="Portrait of Rishab Jain">
  <div class="profile-meta">
    <h1>Rishab Jain</h1>
    <p class="tagline">Student Researcher · {{ site.author.location }}</p>
    <ul class="socials" aria-label="Contact and profile links">
      <li>
        <a href="#" id="email-link" data-u="cmlzaGFiamFpbjEweA==" data-d="Z21haWwuY29t" aria-label="Email">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true" focusable="false"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22 6 12 13 2 6"/></svg>
        </a>
      </li>
      <li>
        <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}/" rel="me" aria-label="LinkedIn">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true" focusable="false"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-4 0v7h-4V9h4v1.6A6 6 0 0 1 16 8z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        </a>
      </li>
      <li>
        <a href="https://github.com/{{ site.author.github }}" rel="me" aria-label="GitHub">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true" focusable="false"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
        </a>
      </li>
    </ul>
  </div>
</section>

Hi! I'm a high school researcher with an interest in computational policy and AI governance in criminal justice + education.

At the moment, I'm conducting research as a [Non-Trivial Fellow](https://www.non-trivial.org/) applying causal inference to understand the heterogeneous treatment effects of educational interventions on juvenile justice contact. I previously [authored an approach](https://doi.org/10.65161/recjcEC1tRGOPCFdc) to revealing and mitigating racial biases in criminal recidivism prediction using a joint-framework of adversarial learning and SHAP.

Outside of research, I have served as the sole student board member on the Fremont Unified School District Board of Education, representing 32,000+ students, and co-founded the [California Student Board Member Association](https://www.csbma.org/Home) to build a state-wide network of youth leaders. I compete in Parliamentary Debate, lead a Scout troop of 50+, and serve as a youth attorney at my local peer court.

## Latest

<ul class="news">
  <li><span class="date">May 2026</span><span>Excited to announce I've been accepted for the <a href="https://www.non-trivial.org/">Non-Trivial Research Fellowship</a> (&lt;2.5% acceptance)! Learn more about my project <a href="{{ '/projects/' | relative_url }}">here</a>.</span></li>
  <li><span class="date">Apr 2026</span><span>My paper, <a href="https://doi.org/10.65161/recjcEC1tRGOPCFdc">"Exploring Bias in Recidivism Prediction via Adversarial Learning and Shapley values"</a> was published in the Oxford Journal of Student Scholarship!</span></li>
  <li><span class="date">Apr 2026</span><span>Founded the <a href="https://www.csbma.org/Home">California Student Board Member Association</a>, a state-wide network for student trustees.</span></li>
  <li><span class="date">Jan 2026</span><span>Earned an auto-qualification bid for the <a href="https://parliamentarydebate.org/">National Parliamentary Debate League</a> Tournament of Champions.</span></li>
  <li><span class="date">Sep 2025</span><span>Joined the <a href="https://nsbma.net/">National Student Board Member Association</a> as Western Regional Strategy Coordinator.</span></li>
</ul>

<script>
  (function () {
    var a = document.getElementById('email-link');
    if (!a) return;
    a.addEventListener('click', function (e) {
      e.preventDefault();
      window.location.href = 'mailto:' + atob(a.dataset.u) + '@' + atob(a.dataset.d);
    });
  })();
</script>

