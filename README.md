# Flixter app 
Flixter is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED (10pts)

- [x] (8pts) Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a separate activity.
- [x] (2pts) Allow video posts to be played in full-screen using the YouTubePlayerView.

#### BONUS

- [ ] Implement a shared element transition when user clicks into the details of a movie (1 point).
- [ ] Trailers for popular movies are played automatically when the movie is selected (1 point).
  - [ ] When clicking on a popular movie (i.e. a movie voted for more than 5 stars) the video should be played immediately.
  - [ ] Less popular videos rely on the detailed page should show an image preview that can initiate playing a YouTube video.
- [ ] Add a play icon overlay to popular movies to indicate that the movie can be played (1 point).
- [ ] Apply data binding for views to help remove boilerplate code. (1 point)
- [ ] Add a rounded corners for the images using the Glide transformations. (1 point)

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

#### REQUIRED (10pts)
- [x] (10pts) User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.

#### BONUS
- [x] (2pts) Views should be responsive for both landscape/portrait mode.
   - [x] (1pt) In portrait mode, the poster image, title, and movie overview is shown.
   - [x] (1pt) In landscape mode, the rotated alternate layout should use the backdrop image instead and show the title and movie overview to the right of it.

- [ ] (2pts) Display a nice default [placeholder graphic](https://guides.codepath.org/android/Displaying-Images-with-the-Glide-Library#advanced-usage) for each image during loading
- [ ] (2pts) Improved the user interface by experimenting with styling and coloring.
- [ ] (2pts) For popular movies (i.e. a movie voted for more than 5 stars), the full backdrop image is displayed. Otherwise, a poster image, the movie title, and overview is listed. Use Heterogenous RecyclerViews and use different ViewHolder layout files for popular movies and less popular ones.

### App Walkthough GIF
<img src="https://i.imgur.com/ygMWK2M.gif" width=250><br>

### Notes
I faced a few challenges while developing my Flixter application. The first one I faced was trying to set up the Glide library in Android Studios and trying to render the book images to the RecyclerView. I have limited experience with Android Studios so I had some trouble trying to import the Glide libray into the program and trying to configure the modules so my android emulator would run without any errors. I was able to solve this problem by referencing the Glide instructions documentation and just tickering around with the modules and 'dependencies' until I was able to get it.

The second problem I was faced was not being able to get my book images to render in the application when running the emulator. This problem was linked to my intial problem because I did not add the dependencies necessary to be able to execute Glide. 

The last issue I encountered was getting my android emulator to display the "horizontal layout view". When I initially ran the emulator and tried to rotate the screen orientation to landscape, the Flixter app would not switch to landscape layout and would just simply stay in the portrait layout even while the emulated phone was rotated. I knew this had nothing to do with my code because I tried running the application on a real physical android Galaxy Note phone and it was able to switch between the views with no problems. I was able to solve this problem because I realized "auto screen rotate" in the emulator settings was not enabled so it would just stay in portrait view for the whole life cycle. After I enabled it I was able to run the landscape layout view. 

### Open-source libraries used

- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Androids
