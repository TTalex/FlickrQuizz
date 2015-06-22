##Introduction
FlickrQuizz is a web-based game using Flickr and Google APIs where the player has to guess locations of random pictures within a city.

An initial configuration allows the player to:
* Select the city he wants to play within
* Use a specific seed if he wants to challenge his friends on the same set of pictures
* Select a preferred game mode, endless continues until the player makes too many errors in a row, the other modes limit the number of pictures
* 
##Used API
* [Flickr API](https://www.flickr.com/services/api/) to retrieve random pictures with geo tags.
* [Google Maps API](https://developers.google.com/maps/) to display a map of the selected city.
* [Google Maps Geolocation API](https://developers.google.com/maps/documentation/geolocation/) to translate city names into latitude and longitude values.

##Installation
1. Make sur Golang is installed
2. Clone the repo

  ```
  git clone https://github.com/TTalex/FlickrQuizz.git
  ```
  
3. Set up the $GOPATH environement variable

  ```
  export GOPATH=`pwd`/FlickrQuizz
  ```

4. Put your own API keys in the source files

##Running it
1. Run the webserver

  ```
  cd FlickrQuizz/src/FlickrQuizz
  go run flickrquizz.go
  ```
  
2. Access [localhost:8081](http://localhost:8081)
