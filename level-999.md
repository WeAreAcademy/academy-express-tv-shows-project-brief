# Level 999 - Misc ideas for further work

This is not really a level at all.

Instead here are some ideas for consideration for further work.

You are free to choose which of these you pursue - just be careful not to let one team member excitedly bring further complexity into an app that is already "enough" for other team members.

-   Allow user to mark (and unmark) "favourite" episodes and favourite shows, and to list only their favourites.
-   Allow user to store their notes about each episode
-   Allow the user to choose to have the show list sorted by rating (highest rated shows first)
-   Add cast listing to your show listing, http://api.tvmaze.com/shows/1?embed=cast
-   Add cast listing to your episode listing, http://api.tvmaze.com/shows/1?embed=cast
-   Allow clicking a cast member to present a view of all shows the person has appeared in http://api.tvmaze.com/people/1/castcredits
    -   linking those back into your episodes view of each show.
-   Truncate long summaries and provide a "... read more..." control to reveal more.
-   Have your search support start-of-word search, or other search types.
-   Use local storage to cache the above
-   Paginate through results with a "load more" button - don't load 100s of episodes at a time.
-   Handle errors gracefully from fetch, letting the user know that something went wrong outwith their control, and that they should try again later (or to select a different show, if appropriate)
-   Responsive design
-   Semantic HTML
-   Accessibility
-   Style your page to fit the theme of the show (colours, typography, background images, etc). Commit to one show to do this.
-   Add a season selector (see screenshot below)

Screenshot of a possible season selector layout for a specific show - you would click to load episodes for the season.

[Example of a possible "season selector" layout](./example-screenshots/example-season-selector.jpg)

[<< level 500](./level-500.md) - [top](./readme.md)
