# BunnyStream-MediaSync
RockRMS plugin for syncing media from BunnyStream (Bunny.net) to RockRMS's Media Accounts.

*_This is under development._* Run at your own risk. I recommend thoroughly testing on a non-production instance of Rock.

Sign up for BunnyStream: [Bunny.net](https://bunny.net?ref=nzxn0bwl71) - I was able to claim 2 week trial and $50 in trial credit.

## Why Does This Exist?
You might think, my videos are on YouTube, or Vimeo, or Resi, or ... why this? I heard rumors that with Vimeo's acquisition they are doing account audits and will likely be forcing many accounts to upgrade. Churches are big bandwidth users and who knows what that will mean for cost. Their CDN is good, but you're bound to their TOS and we're all probably doing some things that push those TOS to the limits.

I know there are other providers that have excellent CDNs, providing on the fly transcoding, have great support, and offer other cool features. So this is one step in the direction of owning your own stuff. No ads, no related videos.

## Who is Bunny.net?
I'll be honest, before today, I had never heard of them. But they popped to the top in search results and in AI recommendations. I compared them to a few other platforms and was pleasantly surprised at the affordability. It's truly consumption based and you get to control all of the levers. They offer georeplication, pop caching, and the coolest feature to me was adaptive HLS stream which is CRAZY fast. Again, you get to control the CDN and not leave it to YouTube or Vimeo. They do a limited trial and you can get $50 credit for two weeks of testing to see if you like it.

## What does this plugin do?
I tried to emulate the way Triumph created the Vimeo Media Sync plugin to a certain degree. What I couldn't pull from BunnyStream I pulled from Rock interactions. In essence, you create a collection in BunnyStream and those videos can be brought in as media elements in Rock. You can then use the Media Shortcode or media lava to show the videos wherever you need them. You can also use it to populate content channels. Just like all other media accounts. 

## Installation
* Set up your [Bunny.net](https://bunny.net?ref=nzxn0bwl71)
* Download the .dll from this repo and drop it into you wwwroot/Bin folder. Note: touching DLLs will cause an AppPool recycle.
* Once your App comes back up, go to Admin Tools > Media Accounts.
* Add a new media account and choose the BunnyStream Media Sync account type.
* You'll need to grab your video library Id and your API key (I recommend read only).
* That's pretty much it. It otherwise operates the same as the other media sync plugins.

## Issues:
* Feel free to post any issues to the GitHub repo and I'll see if I can figure it out.
