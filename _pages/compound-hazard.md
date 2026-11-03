---
permalink: /compound-hazard/
title: "Tropical cyclone hazards and economic losses in coastal North Carolina"
layout: default
author_profile: false
---

{% capture img %}{{ base_path }}/images/papers/compound-hazard{% endcapture %}

<div class="home-wrapper paper">

  <p class="paper-kicker">Working paper, under review</p>
  <h1 class="page__title paper-title">Tropical cyclone hazards and economic losses in coastal North Carolina</h1>

  <p class="paper-authors">
    <span class="pub-self">Jiahang He</span>, Jackson Parker, Brian Blanton, Christine Szpilka, Dahui Liu,
    Kendra Dresback, Randall Kolar, Brian Colle, Linda Nozick, and Ian Sue Wing
  </p>

  <p class="paper-links">
    <a href="https://www.researchsquare.com/article/rs-10540460/v1">Preprint on Research Square</a>
    <span class="paper-sep">&middot;</span>
    <a href="{{ base_path }}/files/compound_hazard_7_30.pdf">PDF</a>
    <span class="paper-sep">&middot;</span>
    <a href="{{ base_path }}/research/">All research</a>
  </p>

  <ul class="stat-row">
    <li><span class="stat-num">575,453</span><span class="stat-label">single-family homes</span></li>
    <li><span class="stat-num">$443 billion</span><span class="stat-label">in residential value</span></li>
    <li><span class="stat-num">604</span><span class="stat-label">synthetic cyclones</span></li>
    <li><span class="stat-num">250 m</span><span class="stat-label">hazard resolution</span></li>
  </ul>

  <div class="page__content">

    <h2>In one paragraph</h2>
    <p>
      Hurricanes hurt coastal regions three ways at once, with wind, storm surge, and inland
      flooding, yet risk assessments usually score each hazard on its own and stop short of
      asking what happens to individual buildings. This paper runs 604 synthetic storms over
      every single-family home in eastern North Carolina, resolves all three hazards at 250-metre
      resolution, and converts them into building-level dollar losses. Separating how many homes a
      hazard reaches from how badly it hits them reveals an imbalance: wind touches most homes but
      does little damage per event, while compound events are rare and six to nine times more
      severe. The compound losses fall disproportionately on homes without insurance.
    </p>

    <h2>Abstract</h2>
    <p class="paper-abstract">
      Tropical cyclones threaten coastal regions through wind, storm surge, and inland flooding,
      yet risk assessments treat these hazards separately and rarely translate them into
      building-level losses. We pair 575,453 single-family homes ($443 billion) in eastern North
      Carolina with a 604-storm synthetic cyclone ensemble and physics-based models resolving wind,
      surge, and flood fields at 250-m resolution, translated to building-level damages. Separating
      each hazard's footprint from its severity reveals a systematic imbalance: wind reaches 62.9%
      of homes but is mild per event (5.1% mean loss ratio), whereas compound events are rare
      (0.19% of building-storm records) yet six to nine times more severe and contribute 9.4% of
      ensemble losses. Wind + flood compounds trace inland riverine corridors missing from
      surge-focused maps, and because they arise from spatial co-occurrence across the regional
      portfolio rather than additive damage at single structures, they undermine the
      diversification underpinning catastrophe insurance. The result is a protection gap: only
      34.6% of homes carry wind and 10.2% flood coverage, over half of worst-case losses fall on
      the uninsured, and every home that cannot afford full coverage is compound-exposed. Those
      most in need of protection are least likely to obtain it.
    </p>

    <h2>How the losses are modeled</h2>
    <figure class="paper-figure">
      <a href="{{ img }}/fig1-framework.webp">
        <img src="{{ img }}/fig1-framework-800.webp"
             srcset="{{ img }}/fig1-framework-800.webp 800w, {{ img }}/fig1-framework.webp 1600w"
             sizes="(max-width: 900px) 94vw, 860px"
             alt="Modeling workflow, synthetic cyclone tracks across the western North Atlantic, and the eastern North Carolina study domain"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        Synthetic storm tracks feed a parametric wind model, a parametric rainfall model routed
        through a hydrologic model, and a dynamical surge model. The resulting wind speeds and
        water depths are matched to every home in the inventory and converted to dollar damage
        with Hazus fragility functions, then passed to an insurance market model. Panel b shows
        the 604 tracks coloured by peak wind; panel c the study domain with its river network.
      </figcaption>
    </figure>

    <h2>Where compound losses land</h2>
    <figure class="paper-figure">
      <a href="{{ img }}/fig5-loss-maps.webp">
        <img src="{{ img }}/fig5-loss-maps-800.webp"
             srcset="{{ img }}/fig5-loss-maps-800.webp 800w, {{ img }}/fig5-loss-maps.webp 1600w"
             sizes="(max-width: 900px) 94vw, 720px"
             alt="Three maps of eastern North Carolina showing the share of census-block losses from wind, surge and flood at the median, 95th and 99th percentile storm"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        Each census block is coloured by the mix of hazards behind its loss: cyan for wind,
        yellow for surge, magenta for flood, blends for compounds. At the median storm (a) wind
        dominates and losses are small. At the 95th (b) and 99th (c) percentiles, wind + flood
        compounds light up the inland river corridors of the Neuse, Tar and Cape Fear, far from
        the coast that surge-focused maps emphasise.
      </figcaption>
    </figure>

    <h2>How intensity compounds</h2>
    <figure class="paper-figure">
      <a href="{{ img }}/fig4-compound.webp">
        <img src="{{ img }}/fig4-compound-800.webp"
             srcset="{{ img }}/fig4-compound-800.webp 800w, {{ img }}/fig4-compound.webp 1600w"
             sizes="(max-width: 900px) 94vw, 720px"
             alt="Heat maps of exposed population, exposed assets and loss across wind speed and inundation depth for wind plus flood and wind plus surge events"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        Joint distributions over wind speed and water depth. Wind + surge (b) is compact: surge
        needs sustained onshore wind, so both peak together at landfall and losses climb steeply
        with wind. Wind + flood (a) is dispersed, because rainfall takes hours to days to route
        through rivers and floods places the strongest winds never reached. Same storm, two
        different physical mechanisms, two different adaptation answers.
      </figcaption>
    </figure>

    <h2>What it means for insurance</h2>
    <figure class="paper-figure">
      <a href="{{ img }}/fig6-insurance.webp">
        <img src="{{ img }}/fig6-insurance-800.webp"
             srcset="{{ img }}/fig6-insurance-800.webp 800w, {{ img }}/fig6-insurance.webp 1600w"
             sizes="(max-width: 900px) 94vw, 860px"
             alt="Maps of coastal North Carolina pricing zones showing wind and flood policy uptake, the uninsured share, equilibrium premiums, and uninsured expected and tail losses"
             loading="lazy" decoding="async">
      </a>
      <figcaption>
        A competitive insurance market simulated for 196,619 coastal homes. Wind coverage reaches
        a third of homes; flood coverage one in ten. Premiums run two to four times expected loss,
        and the loading rises with risk, so the most exposed zones pay the most. Expected uninsured
        loss (f) is a few percent of home value; the 95th-percentile tail (g) is an order of
        magnitude larger, and it concentrates exactly where wind and water converge.
      </figcaption>
    </figure>

    <h2>Takeaways</h2>
    <ul class="paper-takeaways">
      <li>
        Footprint and severity pull in opposite directions. Wind reaches 62.9% of homes with a
        5.1% mean loss ratio; compound events touch 0.19% of building-storm records yet cause 9.4%
        of ensemble losses. The first says where to invest, the second says how much protection
        is needed.
      </li>
      <li>
        Compound exposure is not bad luck. Buildings at the intersection of hazards face
        occurrence probabilities two to two-and-a-half times those of single-hazard structures,
        storm after storm.
      </li>
      <li>
        Compounding is a portfolio problem. Losses compound through co-occurrence across the
        region rather than stacking at single buildings, which erodes the geographic
        diversification that catastrophe insurance relies on.
      </li>
      <li>
        Policy design alone does not close the gap. A combined wind + flood policy lowers
        worst-case uninsured losses only from 59.8% to 54.1% of exposed value, and every home
        that cannot afford full coverage under a 5% premium cap is compound-exposed.
      </li>
    </ul>

    <h2>Cite</h2>
    <p class="paper-cite">
      He, J., J. Parker, B. Blanton, C. Szpilka, D. Liu, K. Dresback, R. Kolar, B. Colle,
      L. Nozick, and I. Sue Wing. Tropical cyclone hazards and economic losses in coastal North
      Carolina. Under review. Preprint:
      <a href="https://www.researchsquare.com/article/rs-10540460/v1">researchsquare.com/article/rs-10540460/v1</a>.
    </p>

  </div>
</div>
