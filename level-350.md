# Level 350 - Switch to fetching _live_ data!

(This is a short level to help you transition to using live data.)

**Pre-req**: For this level you will need to use `axios.get` (or `fetch`) to `GET` JSON content from an API.

## Requirements

1. Complete all minimal requirements from previous levels
1. When your page loads, it must load the episodes (for the SAME show) live from TVMaze API, using axios, instead of importing from the static local data file. (See below for the API "endpoint" (URL) to fetch.)
1. Your search (and episode selector, if you have one) must continue to work as specified in level 300.

## Note on fetching the list of episodes

To get the episodes for the Game of Thrones TV show, you would make an HTTP GET request for this URL: `https://api.tvmaze.com/shows/82/episodes`, using `axios.get` or `fetch`.

similarly, the simpsons data is available at

`https://api.tvmaze.com/shows/82/episodes``

## Learn about the API from its documentation

You can see that this "endpoint" has been documented here: https://www.tvmaze.com/api#show-episode-list

## Loading a different show - just for fun

From the documentation above you can see that the show id is mentioned in the URL.

Try changing that number and obtaining an episode list for other tv shows.

Examples:

-   https://api.tvmaze.com/shows/82/episodes - Game Of Thrones
-   https://api.tvmaze.com/shows/527/episodes - The Sopranos
-   https://api.tvmaze.com/shows/22036/episodes - Planet Earth II
-   https://api.tvmaze.com/shows/5/episodes - True Detective
-   https://api.tvmaze.com/shows/582/episodes - Fresh Prince
-   https://api.tvmaze.com/shows/179/episodes - The Wire
-   https://api.tvmaze.com/shows/379/episodes - Mythbusters
-   https://api.tvmaze.com/shows/4729/episodes - Scrapheap Challenge

[<< level 300](./level-300.md) - [top](./readme.md) - [level 400 >>](./level-400.md)
