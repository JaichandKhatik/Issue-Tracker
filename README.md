# Issue-Tracker

The Search API is optimized to help you find the specific item you’re looking for (e.g., a specific user, a specific file in a repository, etc.). Think of it the way you think of performing a search on Google. It’s designed to help you find the one result you’re looking for (or maybe the few results you’re looking for). Just like searching on Google, you sometimes want to see a few pages of search results so that you can find the item that best meets your needs. To satisfy that need, the GitHub Search API provides up to 1,000 results for each search.

The Search API has a custom rate limit. For requests using Basic Authentication, OAuth, or client ID and secret, you can make up to 30 requests per minute. For unauthenticated requests, the rate limit allows you to make up to 10 requests per minute.

Find repositories via various criteria. This method returns up to 100 results per page.

GET /search/repositories

Suppose we want to search for popular Tetris repositories written in Assembly. Our query might look like this.

https://api.github.com/search/repositories?q=tetris+language:assembly&sort=stars&order=desc


Find issues by state and keyword. (This method returns up to 100 results per page.)

GET /search/issues

Our query might look like this.
"https://api.github.com/repos/" + url+ "/issues?state=all&per_page=100&page=" +pageNo


