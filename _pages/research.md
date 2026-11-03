---
permalink: /research/
title: "Research"
layout: default
author_profile: false
---

{% capture img %}{{ base_path }}/images/papers{% endcapture %}

<div class="home-wrapper">
  <h1 class="page__title">Research</h1>

  <div class="page__content">
    <p>
      I study the economics of climate risk: how tropical cyclones and extreme flooding
      translate into mortality, economic loss and social burden, and how households and
      regional economies adapt afterwards. My work pairs general equilibrium modeling with
      parcel- and household-level data, tracing disaster impacts through the channels that
      actually carry them: infrastructure failure, heat, power outages and healthcare
      disruption.
    </p>

    <h2>Working Papers</h2>
    <p class="wp-lede">Papers under review, and projects at an earlier stage.</p>

    <p class="wp-group">Under review</p>

    <article class="wp">
      <h3 class="wp-title">Tropical cyclone hazards and economic losses in coastal North Carolina</h3>
      <p class="wp-with">
        with J. Parker, B. Blanton, C. Szpilka, D. Liu, K. Dresback, R. Kolar, B. Colle,
        L. Nozick, and <a href="https://www.bu.edu/earth/profiles/ian-sue-wing/">I. Sue Wing</a>
      </p>
      <p class="wp-pill-line"><span class="wp-pill">Under review</span></p>

      <details class="wp-abstract">
        <summary>Abstract</summary>
        <div class="wp-abstract-body">
          <p>
            Tropical cyclones threaten coastal regions through wind, storm surge, and inland
            flooding, yet risk assessments treat these hazards separately and rarely translate
            them into building-level losses. We pair 575,453 single-family homes ($443 billion)
            in eastern North Carolina with a 604-storm synthetic cyclone ensemble and
            physics-based models resolving wind, surge, and flood fields at 250-m resolution,
            translated to building-level damages. Separating each hazard's footprint from its
            severity reveals a systematic imbalance: wind reaches 62.9% of homes but is mild per
            event (5.1% mean loss ratio), whereas compound events are rare (0.19% of
            building-storm records) yet six to nine times more severe and contribute 9.4% of
            ensemble losses. Wind + flood compounds trace inland riverine corridors missing from
            surge-focused maps, and because they arise from spatial co-occurrence across the
            regional portfolio rather than additive damage at single structures, they undermine
            the diversification underpinning catastrophe insurance. The result is a protection
            gap: only 34.6% of homes carry wind and 10.2% flood coverage, over half of worst-case
            losses fall on the uninsured, and every home that cannot afford full coverage is
            compound-exposed. Those most in need of protection are least likely to obtain it.
          </p>
          <figure class="wp-figure">
            <img src="{{ img }}/compound-hazard/fig1a-workflow-800.webp"
                 srcset="{{ img }}/compound-hazard/fig1a-workflow-800.webp 800w, {{ img }}/compound-hazard/fig1a-workflow.webp 1280w"
                 sizes="(max-width: 900px) 94vw, 820px"
                 alt="Workflow diagram of the compound hazard modeling chain, from synthetic storm tracks through wind, surge and flood models to building losses and the insurance model"
                 loading="lazy" decoding="async">
            <figcaption>
              The modeling chain: synthetic storm tracks drive wind, rainfall-to-flood and
              surge models; the resulting hazards are matched to every home and converted to
              losses, which feed an insurance market model.
            </figcaption>
          </figure>
        </div>
      </details>

      <p class="wp-links">
        <a href="https://www.researchsquare.com/article/rs-10540460/v1">Preprint</a>
        <a href="{{ base_path }}/files/compound_hazard_7_30.pdf">PDF</a>
      </p>
    </article>

    <p class="wp-group">In progress</p>

    <article class="wp">
      <h3 class="wp-title">Tropical cyclone mortality mechanisms: infrastructure failure, heat, power outages, and healthcare disruption</h3>
      <p class="wp-with">with <a href="https://www.bu.edu/earth/profiles/ian-sue-wing/">I. Sue Wing</a></p>
      <p class="wp-pill-line"><span class="wp-pill">Draft in progress</span></p>
    </article>

    <article class="wp">
      <h3 class="wp-title">Economy dynamics and disaster resilience for households in North Carolina: an adaptive rolling intertemporal planning model</h3>
      <p class="wp-with">with <a href="https://www.bu.edu/earth/profiles/ian-sue-wing/">I. Sue Wing</a></p>
      <p class="wp-pill-line"><span class="wp-pill">Draft in progress</span></p>
    </article>

    <article class="wp">
      <h3 class="wp-title">Household sorting over tropical cyclones in North Carolina</h3>
      <p class="wp-pill-line"><span class="wp-pill">Early stage</span></p>
    </article>

    <article class="wp">
      <h3 class="wp-title">A parcel-level implementation of the capabilities-approach social burden metric for Massachusetts coastal communities</h3>
      <p class="wp-with">with <a href="https://innsure.org/">InnSure</a></p>
      <p class="wp-pill-line"><span class="wp-pill">Draft in progress</span></p>
    </article>

  </div>
</div>
