---
layout: page
title: Search
---

<div id="search-container">
  <input type="text" id="search-input" placeholder="Type here...">
    <ul id="results-container" class="tags-expo-posts"><small>Start typing to see some results</small></ul>
</div>

<script src="/assets/js/jekyll-search.js" type="text/javascript"></script>
<script type="text/javascript">
  SimpleJekyllSearch.init({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    dataSource: '{{ site.baseurl }}/search.json',
    searchResultTemplate: '<li class="post-title"><a href="{url}" title="{desc}">{title}<\/a><\/li>',
    noResultsText: 'No results found',
    limit: 10,
    fuzzy: true,
  })
</script>
