# j5-songs [![Build Status](https://secure.travis-ci.org/julianduque/j5-songs.png?branch=master)](http://travis-ci.org/julianduque/j5-songs)

Songs for Johnny-Five Piezo class

## Getting Started
Install the module with: `npm install j5-songs --save`

```javascript
var five = require('johnny-five');
var songs = require('j5-songs');

five.Board().on('ready', function () {
  var piezo = new Piezo();

  // Load a song object
  var song = songs.load('never-gonna-give-you-up');
  
  // Play it !
  piezo.play(song);

  // List all songs
  songs.list(function (err, tunes) {
    // Object literal with all the songs
  });
});
```

## Songs

| Song ID                 | Artist      | Name                    |
|-------------------------|-------------|-------------------------|
| never-gonna-give-you-up | Rick Astley | Never Gonna Give You Up |


## License
Copyright (c) 2014 Julian Duque. Licensed under the MIT license.
