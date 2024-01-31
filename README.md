# Academy Project: TV Shows

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

## Overview

You must make an Express web app which shows details of all of the episodes of a TV show.

The episode data will come from [TV Maze](http://www.tvmaze.com/).

Later iterations of your app will add other features such as allowing the user to "favourite" certain episodes or certain shows.

## About the episode data

### Where do I get the episode data from?

The episode data will come from [TV Maze](http://www.tvmaze.com/).

Initially, you'll use the data that's already been saved for you into the starter repo. This was obtained by manually saving data from their [API](http://www.tvmaze.com/api) (specifically [this link](https://api.tvmaze.com/shows/82/episodes)).

In later exercises you will be challenged to have your app dynamically `fetch` the data from the API.

In all cases, you will be working with an array of objects, each of which represents an episode of a TV show, with properties that include the title, runtime, and summary of the episode.

### What does the episode data look like?

Here's an excerpt of [this file](https://api.tvmaze.com/shows/82/episodes) showing an example of ONE episode from the list. It's a lot. You won't need all of the fields!

```js
{
    id: 4952,
    url: "https://www.tvmaze.com/episodes/4952/game-of-thrones-1x01-winter-is-coming",
    name: "Winter is Coming",
    season: 1,
    number: 1,
    type: "regular",
    airdate: "2011-04-17",
    airtime: "21:00",
    airstamp: "2011-04-18T01:00:00+00:00",
    runtime: 60,
    rating: { average: 8.4 },
    image: {
      medium:
        "https://static.tvmaze.com/uploads/images/medium_landscape/1/2668.jpg",
      original:
        "https://static.tvmaze.com/uploads/images/original_untouched/1/2668.jpg",
    },
    summary:
      "<p>Lord Eddard Stark, ruler of the North, is summoned to court by his old friend, King Robert Baratheon, to serve as the King's Hand. Eddard reluctantly agrees after learning of a possible threat to the King's life. Eddard's bastard son Jon Snow must make a painful decision about his own future, while in the distant east Viserys Targaryen plots to reclaim his father's throne, usurped by Robert, by selling his sister in marriage.</p>",
    _links: { self: { href: "https://api.tvmaze.com/episodes/4952" } },
}
```

## Setup

Select one of your team to own your repo.

Make a new repo from the following starter code by clicking "Use as template" in github.
[https://github.com/WeAreAcademy/academy-express-tv-shows-project-starter/](https://github.com/WeAreAcademy/academy-express-tv-shows-project-starter/)

-   Set up continuous deployment of your app to [Render.com](https://render.com) as, for example, `academy-yourteamname-tv-shows`.onrender.com.

### Setup - get the episode data if required

-   The starter app should already have the episode data for the show "Game Of Thrones" from TV Maze API. If it does not, download it using this URL:
    https://api.tvmaze.com/shows/82/episodes

-   Save the file as `src/data/gameOfThrones.js` in your project's `src` directory, and modify the file to export the content as an array, called gameOfThronesEpisodes.

-   Import the JSON data into a variable at the top of your `app.js` as follows:

`const {gameOfThronesEpisodes} from './data/gameOfThronesData.js'`

-   Check the import was successful by adding the following after the import and checking the browser's console when the app loads.

```
console.log(`Imported ${gameOfThronesEpisodes.length} episode(s)`);
console.log(`First episode's name is ${gameOfThronesEpisodes[0].name}`);

Note: For those wanting to use JSDoc, a naive type-definition of an episode object has been provided and imported into app.js.  It includes some intentional imperfections which you may need to address later in the project, but it should be fine to get started with.

```

### Rules about the episode data

You MUST NOT edit the static episode data. If you find that the data is unsuitable (e.g. fields are missing, or have unwanted characters), you should improve your own code so that _it_ can deal with such issues at run-time.

Why? If your app is later extended to allow the downloading of episode data for any one of hundreds of possible shows, frequently updated, tidying the data by hand will NOT be a feasible solution! It's important to practice thinking about - and writing code to help with - the handling of inconsistencies in data.

## Project Levels

This project is broken into various levels:

-   [level 100](./level-100.md)
-   [level 200](./level-200.md)
-   [level 300](./level-300.md)
-   [level 350](./level-350.md)
-   [level 400](./level-400.md)
-   [level 500](./level-500.md)
-   [level 999 (further work)](./level-999.md)
