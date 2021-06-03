# What's Your Troubleshooting Process?

*This [blog post][1] originally appeared on the* ProfHacker *blog at the* Chronicle of Higher Education *on July 18, 2011.*

![][image-1]

A little over a week ago, I hit a snag with my three year-old MacBook. I wanted to test the Hangouts feature in Google Plus---and discovered that the built-in iSight camera wasn’t working. A quick check showed that it wasn’t working with \_any\_application; Skype and Photo Booth also refused to talk to the camera, with Photo Booth going so far as to tell me that I didn’t even have a camera connected.

I wasn’t too concerned at first. Like many users, I’ve occasionally experienced the problem of the camera’s light coming on during bootup, and the camera then refusing to work. Normally shutting the computer down and pulling the battery, then reinserting the battery and restarting the computer, resolves the problem.

Figuring this issue might be a similar kind of problem, that’s the first thing I did. No luck. Photo Booth still insisted there was no camera connected. Rats. It was a different kind of problem, so I was going to have to do some investigation.

Here’s what I did:

- First, I did some Googling. Were others experiencing the same sort of difficulty? (Yes, as a matter of fact, they were.) My initial search turned up a lot of irrelevant material; restricting the search to forum discussions at [apple.com][2] helped.
- Second, I had to figure out whether the problem was with the camera itself, or lay elsewhere. That entailed reading through a number of forum threads to see how to determine what the problem was most likely to be.
- A look at the information in System Profiler showed that the MacBook could see the camera. That suggested that the problem had something to do with my user profile. To test that hypothesis, I created a new user profile, then logged into it.
- Sure enough, the camera worked just fine in the new user profile. Since I couldn’t figure out what the problem with the profile was or how to fix it, I had to transfer all my files and folders from the old, corrupt profile to the new one. (Restoring from a TimeMachine backup didn’t work, as the profile was corrupted there, too.)
- The transfer process turned out to be more tedious than difficult, at least once I realized that I had to change permissions on those files and folders to make things work.

So, several hours after I first realized I had a problem, I had a new, uncorrupted profile and a working camera.

In the process of sorting out this mess, I made use of some skills I already had, plus I learned a few new things about how OS X handles permissions.

The experience got me to thinking about how I might help students learn, beginning from what they already know. In my case, I already knew how to describe my problem and how to filter search results so I’d be more likely to see things that might actually be helpful in my situation. From there, it was a matter of carefully reading and applying what I read---at least until I ran into the permissions issue, at which point, having encountered a new problem, I repeated the process.

As I’m starting to think more seriously about fall classes, I’m trying to think of some discipline-appropriate classroom activities that will help my students work through a similar process: figuring out what they already know, what they need or want to know, and using the first to help them get to the second.

***What about you — what have been your own experiences of reflecting on your own learning processes, and making use of that reflection in the classroom? Let us know in the comments.***

*[*[*Creative Commons licensed Flickr photo by ehecatzin*][3]*]*


[1]:	http://chronicle.com/blogs/profhacker/whats-your-troubleshooting-process/34729
[2]:	http://www.apple.com/
[3]:	http://www.flickr.com/photos/ehecatzin/71173175/

[image-1]:	# "Screenshot of Mac with several communications windows open"