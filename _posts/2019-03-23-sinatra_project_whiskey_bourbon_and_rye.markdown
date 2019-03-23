---
layout: post
title:      "Sinatra Project: Whiskey, Bourbon & Rye!"
date:       2019-03-23 14:54:07 -0400
permalink:  sinatra_project_whiskey_bourbon_and_rye
---


​The biggest challenge with starting a new project is deciding exactly where to begin. I spent the first few days reading every piece of Sinatra literature I could. I needed to reinforce my understanding of several concepts that I struggled with while making the Twitter clone - Fwitter ( 
[https://github.com/brandong1/sinatra-fwitter-group-project-v-000])

My next task was deciding exactly what I wanted to do for my Sinatra project. Fortunately, it didn’t take long for me to come up with the idea of a liquor database. This was inspired by the book, Whiskey Bourbon & Rye by Clay Risen, which I’ve been using to track which spirits I’ve tried and whether I like them or not.

![Imgur](https://i.imgur.com/HIWaZeW.jpg)


I’ve been going through highlighting each drink in the book as I try them and figured creating a website would be a perfect way to digitize my hobby!

It took a few days for me to get on track. I have a terrible habit of researching features that are beyond the requirements of the project. Inevitably, I get stuck in a rabbit hole of possible features I want to add which stalls any actual progress. **FOCUS ON THE REQUIREMENTS AND NOTHING ELSE.** 

Features can be added later!

![Imgur](https://i.imgur.com/AQ3a6fL.jpg)

Well then, here’s an error that annoyed the hell out of me:


![Imgur](https://i.imgur.com/rVM1MLr.jpg?2)


![Imgur](https://i.imgur.com/HGWVn02.jpg?2)
**Note the extra ‘)’ on line 21… took me an hour to notice that..**


After changing my current_user(), and removing the extra parenthese, I finally got my form to display.

![Imgur](https://i.imgur.com/G4FlV6s.jpg?1)

TOTAL TIME SPEND ON TRYING TO GET THIS FORM TO DISPLAY PROPERLY: 4 HOURS!!!! 
I
I’m starting to think this project is going to take forever to finish. (**It did..**)


Next issue I ran into was getting the prices to display properly.

![Imgur](https://i.imgur.com/BLNSI49.jpg?1)

![Imgur](https://i.imgur.com/ReYpkZv.jpg)

YIKES!



After scouring GitHub for a Sinatra project similar to mine, I came across Jeremy Schuurman’s Vino project (https://github.com/JMSchuurmans/vino-sinatra) and seeing how he converted his wine price from float to string made sense because I didn’t care about decimal places in my liquor prices.

![Imgur](https://i.imgur.com/rf0rUIu.jpg?1)


After I created and ran my new migration, I went from Gross to Gucci and earned myself 4oz of Speyburn Scotch! "Once it hits the lips, it’s so good!"

![Imgur](https://i.imgur.com/w90pcwv.jpg?1)

Another issue that gave me trouble for a good three hours was this terrible message when I was trying to get my forms to display:

![Imgur](https://i.imgur.com/2jeLUus.jpg?1)

When I reached my breaking point, I just started deleting and commenting things out one by one until I eventually found the culprit:

![Imgur](https://i.imgur.com/5xwtWFj.jpg?1)

In one of my many “Oh, I should add this cool feature” tangents, I ended up trying to implement flash messages. It didn’t work out so well and honestly, it was distracting me. I commented out everything related to flash messages and boom!

At this point, I just wanted to be done so I’m just sticking to the basics.

My next problem took me several hours to finally figure out. 

![Imgur](https://i.imgur.com/6QBBEeA.jpg?1)

I thought this code was Boss! Using ‘fetch’, which I’ve never done before, but hindsight, I can’t believe how wrong I was. The above code gave me the following error page:

![Imgur](https://i.imgur.com/L9FfJgM.jpg?1)

Three days later… THREE.

![Imgur](https://i.imgur.com/iOtVEV8.jpg?1)

When my edit page finally rendered properly, I felt like a gangsta! 

A web-developing gangsta!

![Imgur](https://i.imgur.com/U2fNZ8U.jpg?1)


I don’t even remember how I got this error, but it was 2am and my eyes started glazing over so it was understandable when I realized I didn’t run bundle install after adding or updating my gemfile.

![Imgur](https://i.imgur.com/IezWb7j.jpg?1)

Enough about all the problems I encountered, let’s talk about the finished product.

**CREATE**
You can create a new user:

![Imgur](https://i.imgur.com/7SlPsFu.jpg?1)

Once the account is created, you can create a new liquor:

![Imgur](https://i.imgur.com/GoZzrCk.jpg?1)

And then you can **READ** that users list of liquors they created:

![Imgur](https://i.imgur.com/oXXzjxG.jpg?1)

Each user can **UPDATE** their own account info and the liquors they created:

Update User account:

![Imgur](https://i.imgur.com/z5r3YEh.jpg?1)

Update user’s liquors:

![Imgur](https://i.imgur.com/EOPGoOb.jpg?1)

And finally, each user can **DELETE** the liquors they’ve created:

![Imgur](https://i.imgur.com/1Jo0T5U.jpg?1)

Overall, I’m happy with how my project turned out and I’m looking forward to adding additional features to this project when I learn Rails.
