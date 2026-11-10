---
layout: page
permalink: /publications/
title: publications
description: publications by category in reversed chronological order.
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h2>First- and Second-Author Publications</h2>

{% bibliography --query @*[keywords=primary] %}

<h2>Contributing-Author Publications</h2>

{% bibliography --query @*[keywords=contributing] %}

</div>
