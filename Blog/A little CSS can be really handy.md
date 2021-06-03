# A little CSS can be really handy

A couple of months ago (February 2021) I started using Ghost as my blogging platform.[^1] I’ve come to like it a lot; it’s easy to use, it’s focused on writing, and it has solid [features][1] for those who write professionally.

One of Ghost’s major features for professional writers is making it easy for readers to sign up for an email newsletter subscription, which can be free or paid. Though it’s a very useful feature, it’s not one that I want to use at this point, so I’d rather hide it from readers (who can always use the built-in [RSS feed][2] if they really want to subscribe).

It’s a simple matter to hide the subscribe button that appears at the lower right of each page; all that’s necessary is to go into Ghost’s portal settings and ensure that “Show Portal button” is toggled off.

For some themes, though, that won’t be sufficient to hide subscription options, and that’s where a little knowledge of CSS can really be handy. I’m using the excellent [Liebling theme][3] by [Eduardo Gómez][4]. It shows information about subscriptions in two places.  Using Chrome’s developer tools, I can inspect the button on the landing page:
![][image-1]

I can also inspect the subscribe section that appears on every post page:
![][image-2]

Then, using the the information gleaned from inspecting those items, I can hide them with just a few lines of code added to the header section in the code injection area of Ghost’s settings:
`<style>  
    .m-button.filled display:none;  
    .m-subscribe-section display:none;  
</style>
`
If I ever decide to make use of the newsletter feature, all I need to do is remove those few lines of code to allow readers to see the option. 

*Photo credit: [Mika Baumeister][5] on [Unsplash][6]*
  

[^1]:	For those who may be wondering: I was using WordPress previously. WordPress is really powerful, and there’s a lot to like about it. I came to the conclusion, though, that it did far more than I needed, and that I’d do well to switch to something that wouldn’t require as much effort to maintain.

[1]:	https://ghost.org/features/
[2]:	https://amycavender.com/rss/
[3]:	https://liebling.eduardogomez.io
[4]:	https://github.com/eddiesigner
[5]:	https://images.unsplash.com/photo-1563206767-5b18f218e8de?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1
[6]:	https://unsplash.com

[image-1]:	# "Using Chrome's developer tools to inspect the subscribe button."
[image-2]:	# "Using Chrome's developer tools to inspect the subscribe section."