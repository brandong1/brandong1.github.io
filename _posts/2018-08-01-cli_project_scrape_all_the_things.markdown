---
layout: post
title:      "CLI Project: Scrape All The Things!"
date:       2018-08-02 00:27:15 +0000
permalink:  cli_project_scrape_all_the_things
---


Two weeks ago, I didn’t even know websites could be “scraped”, yet here I am, on Cloud 9 after creating my first CLI Data Gem.

Truth be told, my time at Flatiron School has been full of frustration and high blood pressure, but there’s no better feeling than running a fully functioning program that you created from scratch.

For my CLI Data Gem Project, I decided to scrape the Hacker News website:  [https://news.ycombinator.com/](https://news.ycombinator.com/) 

Having **BARELY** managed to work my way through the Scraper Lab and Music CLI Library labs, I knew this project would not be easy.

Being part of the beta group for the Structured Online Program has changed my attitude about programming. The first two months of me struggling through the curriculum alone were tough, but having a “cohort” of fellow coders, most of whom seem to be riding the same Struggle Bus as I am, has renewed my motivation to do better. With their support, I’ve made more progress than I would have working solo.

To get started on my project, I ended up watching Avi’s Daily Deal [https://www.youtube.com/watch?v=_lDExWIhYKI ] video as well as my Cohort Instructor’s, walkthrough for creating a CLI Gem from scratch.

I used Cernan’s video to get my initial file structure created using  bundler. From there, it was just a matter of working through my logic.

I started with my CLI, because it was mentally easier for me to work on the program in the order that the user would experience it. It began with my main_menu.

In my cli.rb, when getting the user’s input, I decided to try using case/when instead of `if/else`. As I read more books on Ruby, I’m discovering more and more “syntactic sugar” that I get eager to try.

Instead of having a bunch of `if/else` statements, I put `case/when` to the test:

```
until input == "exit"
            input = gets.strip
            case input.downcase #Input is NOT case sensitive
            when "news"
                puts "========================================".colorize(:red)
                puts "This shows a list of news headlines: "
                HackerNews::Article.list_news 
                #do I need to pass the "type" i.e. news or jobs?
            when "jobs"
                puts "========================================".colorize(:red)
                puts "Here is a list of available jobs: "
                HackerNews::Jobs.list_jobs
            when "exit"
                puts puts "========================================".colorize(:red)
                puts "Have a great day!"
...
...
```

The general consensus on Stack Overflow is that `case/when`  is just a more readable way of expressing the idea.

They did mention that `if/else` is faster than `case/when` because `case` “implicitly compares using the more expensive `===` operator”.
See: [midwife.github.io/blog/2011/08/26/ruby-performance-case-vs-if-else](http://midwife.github.io/blog/2011/08/26/ruby-performance-case-vs-if-else)


Granted, that test is old and may have been addressed in Ruby since then, but either way, `case` offered less typed. “Lazy programmer”, FTW!

# ***Side note***
By the time I got my CLI fully functional, I had over 45 commits! Commit everything!

The biggest challenge I had was getting my #Scraper class method #scrape_news  and #scrape_jobs to scrape the exact data I wanted:

![](https://i.imgur.com/ISmZIhO.png)

I had to request 1:1 assistance to figure it out and the way the tech coach recommended I code it was:

`doc.css('.title a.storylink').each ...`

That was a huge hurdle that I was glad to get over!

I very proud of my progress in the cirriculum!

![](https://i.imgur.com/uLZGLXt.png)


