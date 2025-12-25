---
title: "Editions"
layout: default
permalink: "/editions/"
---

<section class="mt-4 mb-5">
  <div class="container mb-4">
    <h1 class="font-weight-bold title">Benchmark Editions</h1>
    <p class="text-muted">
      Each year is a separate edition of the benchmark suite. Posts under an edition include announcements, downloads,
      rules, datasets, baselines, results, and FAQs.
    </p>

    <div class="row">
      <div class="col-md-12">
        <div class="card border-0 shadow-sm">
          <div class="card-body">
            <h5 class="mb-3">Browse by year</h5>
            <div class="d-flex flex-wrap">
              {% assign years = "2022,2023,2024,2025,2026,2027,2028,2029,2030" | split: "," %}
              {% for y in years %}
                  <a class="btn btn-light mr-2 mb-2" href="{{site.baseurl}}/editions/{{y}}/">{{y}}</a>
              {% endfor %}
            </div>
            <p class="small text-muted mb-0 mt-2">
              Tip: when you create a post, add <code>edition: 2026</code> in its front matter so it shows up under that year.
            </p>
          </div>
        </div>
      </div>
    </div>

    <hr class="my-4"/>

    <h3 class="mb-3">Latest posts across all editions</h3>
    <div class="row">
      {% for post in site.posts limit:12 %}
        {% include card-post.html %}
      {% endfor %}
    </div>

  </div>
</section>
