---
layout: post
title: The World By Cinema
subtitle: A Map of the Best Film Made in Every Country
thumbnail-img: /assets/img/WBC.png
share-img: /assets/img/WBC.png
tags: [film, mapping]
comments: true
author: Luke RF
---

Once upon a time, I used the World Cinema society back in my undergrad Uni. It was often difficult to choose the film of the week to screen - all the films in all the world and I had to choose one that would both attract and satisfy an audience. Needless to say it was imperfect, but I had a good time.

Taking advantage of [TMDB's](https://www.themoviedb.org/?language=en-GB) open movie database, I figured I can pull the best films from any given country. The best way to show geographic information is ... maps. So this is what I did. My friend and comrade [Alfie](https://alifeee.co.uk/) helped me a lot.

[Click here to see the full interactive map!](https://ekulrf.github.io/BestFilmsByCountry/)

<a href="https://ekulrf.github.io/BestFilmsByCountry/">
  <img alt="Best Films By Country" src="/assets/img/WBC.png">
</a>

Issues: 
- the mapping package I used is difficult to manipulate, meaning a lot of the images can't be discerned without hovering over. I'd improve this with a better package but I cba.
- the TMDB database lists 'Country of Origin' as any country used in the production of the film. The result of this is many countries sharing a best film. From this I learned the film [Baraka](https://www.themoviedb.org/movie/14002-baraka) was shot in 24 countries on six continents (a cool fact but annoying here).

Interesting:
- The 'best' film from Bolivia is a sex film called [Mi Prima La Sexóloga](https://www.themoviedb.org/movie/525686-mi-prima-la-sexologa)
- The 'best' film from Portugal is [Barbie as the Island Princess](https://www.themoviedb.org/movie/13283-barbie-as-the-island-princess)
- Making maps, especially when you're interested in countries, is inherently political. Contested borders in and around China, the war in Ukraine, etc. force you to make political statements when making maps - even if unintentional.

You can see the code and everything here if you like (https://github.com/EkulRF/BestFilmsByCountry).