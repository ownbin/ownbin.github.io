---
layout: page
title: Search
---

<div>In case you don't want to use the search box provided by your browser:</div>

<div id="search-container">
  <input type="text" id="search-input" placeholder="Type here...">
</div>
<br/>
<ul id="results-container"><small>Start typing to see some results</small></ul>

<script src="/assets/js/jekyll-search.js" type="text/javascript"></script>
<script type="text/javascript">
  SimpleJekyllSearch.init({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    dataSource: '{{ site.baseurl }}/search.json',
    searchResultTemplate: '<li><a href="{url}" title="{desc}">{title}<\/a><\/li>',
    noResultsText: 'No results found',
    limit: 10,
    fuzzy: true,
  })
</script>
