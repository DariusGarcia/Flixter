# Flixter 
Flixter is a native Android mobile app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED

- [x] Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a separate activity.
- [x] Allow video posts to be played in full-screen using the YouTubePlayerView.

### App Walkthough GIF

<img src="https://i.imgur.com/BmYq5bP.gif" width=250><br>

### Notes

One roadblock I faced while developing this second part of the application was that I could not get the youtube player to correctly show on my app. I was able to solve this issue by making sure to import all the neccessary modules and libraries into my project directory.

## Open-source libraries used
- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Android

---

## Flix Part 1

### User Stories

#### REQUIRED 
- [x]  User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.

#### BONUS
- [x]  Views should be responsive for both landscape/portrait mode.
   - [x]  In portrait mode, the poster image, title, and movie overview is shown.
   - [x]  In landscape mode, the rotated alternate layout should use the backdrop image instead and show the title and movie overview to the right of it.

### App Walkthough GIF
<img src="https://i.imgur.com/ygMWK2M.gif" width=250><br>

### Notes
I faced a few challenges while developing my Flixter application. The first one I faced was trying to set up the Glide library in Android Studios and trying to render the book images to the RecyclerView. 

The second problem I was faced was not being able to get my book images to render in the application when running the emulator. This problem was linked to my intial problem because I did not add the dependencies necessary to be able to execute Glide. 

The last issue I encountered was getting my android emulator to display the "horizontal layout view". When I initially ran the emulator and tried to rotate the screen orientation to landscape, the Flixter app would not switch to landscape layout and would just simply stay in the portrait layout; Even while the emulated phone was rotated. I knew this had nothing to do with my code because I tried running the application on a real physical android Galaxy Note phone and it was able to switch between the views with no problems. I was able to solve this problem because I realized "auto screen rotate" in the emulator settings was not enabled so it would just stay in portrait view for the whole life cycle. After I enabled it I was able to run the landscape layout view. 

### Open-source libraries used

- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Androids
