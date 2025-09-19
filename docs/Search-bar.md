### Searching

The default search setting is to search through all your apps and bookmarks. If you want to search using specific search engine, you need to type your search query with selected prefix. For example, to search for "what is docker" using google search you would type: `/g what is docker`.

You can set which search engine should be the default one. If you set DuckDuckGo as a default search provider you can just type your query without using `/d` prefix. To search and redirect to the results, just press `Enter`.

Search bar will also detect valid URLs and IPs and will redirect directly to them instead of searching.

### Local search
Local search is the default search provider so you don't need to use prefix to search. However, if you change the default search enigne you will need to use `/l` prefix. 

If app or bookmark was found, you can easily open it by pressing `Enter`.

### Adding custom search engine

You can add your own search engines. Go to `Settings > Search` and then add your custom search engine. You will need to provide an unique prefix and search template like `https://duckduckgo.com/?q=` or `https://whoogle.sdf.org/search?q=`. You can also set it to be your default search provider.

### Shortcuts

Search bar supports some shortcuts:
- Focus on the search bar
  - `Esc` - clear input
  - `LMB double click` - clear input
- Focus outside the search bar
  - `Esc` - clear input
  - `backtick` - (`) clear input and focus on the search bar

### Built-in search providers

| Name               | Prefix | Search URL                                    |
|--------------------|--------|-----------------------------------------------|
| Deezer             | /dz    | https://www.deezer.com/search/                |
| Disroot            | /ds    | http://search.disroot.org/search?q=           |
| DuckDuckGo         | /d     | https://duckduckgo.com/?q=                    |
| Google             | /g     | https://www.google.com/search?q=              |
| IMDb               | /im    | https://www.imdb.com/find?q=                  |
| Reddit             | /r     | https://www.reddit.com/search?q=              |
| Spotify            | /sp    | https://open.spotify.com/search/              |
| The Movie Database | /mv    | https://www.themoviedb.org/search?query=      |
| Tidal              | /td    | https://listen.tidal.com/search?q=            |
| Wikipedia          | /w     | https://en.wikipedia.org/w/index.php?search=  |
| YouTube            | /yt    | https://www.youtube.com/results?search_query= |