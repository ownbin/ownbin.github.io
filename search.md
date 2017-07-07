---
layout: page
title: Search
banner_image: sample-banner-image-1.jpg
---
<div class="tags-expo">
  <div class="tags-expo-list">
<span class="octicon octicon-mark-github"></span>
<div id="search-container">
  <input type="text" id="search-input" placeholder="Type here...">
  <div class="tags-expo-section">
    <ul id="results-container" class="tags-expo-posts"><small>Start typing to see some results</small></ul>
  </div>
</div>

  </div>
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
