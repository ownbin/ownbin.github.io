---
layout: page
title: Search
---

<div>Find something quickly, start typing to see some results.</div>
<div id="search-container">
  <input type="text" id="search-input" placeholder="Type here...">
</div>
<!--<ul id="results-container">Start typing to see some results</ul>-->
<div id="results-container"></div>

<script src="/assets/js/jekyll-search.js" type="text/javascript"></script>
<script type="text/javascript">
  SimpleJekyllSearch.init({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    dataSource: '{{ site.baseurl }}/search.json',
    //searchResultTemplate: '<li><a href="{url}" title="{desc}">{title}<\/a><\/li>',
    searchResultTemplate: '<p><a href="{url}" title="{desc}">{title}<\/a><\/p>',
    noResultsText: '<p>No results found</p>',
    limit: 10,
    fuzzy: true,
  })
</script>
