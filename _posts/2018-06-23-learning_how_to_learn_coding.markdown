---
layout: post
title:      "Learning How To Learn Coding"
date:       2018-06-23 18:07:58 +0000
permalink:  learning_how_to_learn_coding
---


It took me a long time to realize I can't learn coding, or anything  for that matter, like everyone else. I especially found this to be true all throughout school.

I get bored listening to someone lecture about a topic. This is the reason why my notes have never been helpful. Combine this with a bit of ADHD and I've got a recipe for disaster.

During these first few months at Flatiron School, I've identified how I learn best:

1) Tell me (briefly) how to do it.

2) Show me how to do it.

3) Let me do it.

For example:
```
class Artist
    ...
   
	 # a method 'add_song_by_name', that takes in an argument of a name and genre and both creates the new song and adds that song to the artist's collection.
	 
    def add_song_by_name(name, genre) 
      song = Song.new(name, genre)
      @songs << song
      song.artist = self # Telling the song object that it belongs to the Artist
    end
```

A simple comment that tells me exactly what that method does is effective enough for me to understand what needs to be done to get the desired results.

```
song.artist = self # Telling the song object that it belongs to the Artist
```

This allows me to break down each line of code by adding my own comments that explains, in my own words, what that line of code does.

I do this even when I'm already familiar with what the line of code does just so I can keep it fresh in my mind and get used to explaining what my code is doing for the benefits of others who read it.

The Flatiron School cirriculum does a great job of introducing the coding concepts to me and getting me in the mindset that even though they give the tools necessary to pass each lab, I have to use other resources to expand my knowledge.

I've found I actually spend more time researching and reading documentation than I do on the Learn platform. 

And maybe that's the point.
