---
layout: page
title: Cari
---

<style>
	#search-container {
	    max-width: 100%;
	}

	input[type=text] {
		font-size: normal;
	    outline: none;
	    padding: 1rem;
		background: #202020;
	    width: 100%;
		-webkit-appearance: none;
		font-family: inherit;
		font-size: 100%;
		border: none;
		border-radius: 6px;
	}
	#results-container {
		margin: .5rem 0;
	}
</style>

<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="Cari ....">
<ol id="results-container"></ol>
</div>

<!-- Script pointing to search-script.js -->
<script src="/search.js" type="text/javascript"></script>

<!-- Configuration -->
<script type="text/javascript">
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/search.json',
  searchResultTemplate: '<li><a href="{url}" title="{description}">{title}</a></li>',
  noResultsText: 'Hasil tidak ditemukan.',
  limit: 10,
  fuzzy: false,
  exclude: ['Welcome']
})
</script>
