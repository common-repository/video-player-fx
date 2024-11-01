=== Video Player FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, video, player, flv, mp3, audio, sound, xml, play, preloader, as3, vertical, horizontal, list, subtitle, full, screen
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

Probably the most advanced, flexible, customizable and easy to use audio/video player without any Flash knowledge. And it's free!

== Description ==

This high customizable video/audio player can be embedded in any website for free without any Flash knowledge. It can have an overall width and height up to 1680 x 1050 pixels and supports fullscreen mode. It has over 100 customizable properties which can be modified using just a settings.xml file. You can insert your own subtitles for videos, the text being easy customizable using a style.css file. You can also set your desired watermark and a starting image for each video/audio item. The player is fully skinnable through a xml file, using external images this way each button can be personalized. The buttons for video/audio controll can be rearranged in any order and also enabled/disabled. It also has a scrollable list, xml customizable, for media content. Each item from the list can have a description and a thumb.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/video-player-fx.zip "Video Player FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/video-player.zip "Video Player FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **video-player-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Video Player FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[video-player-fx][/video-player-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Video Player FX part of your theme, edit the template files and add `<?php videoplayerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Video Player FX](http://www.flashxml.net/video-player.html "Video Player FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/video-player-fx/settings.xml`
7. To use your own videos, upload them to `wp-content/flashxml/video-player-fx/video/` and update the `wp-content/flashxml/video-player-fx/media.xml` file accordingly

= Additional settings file =

To embed the Video Player FX more than once, you will need another settings file and (probably) another set of videos. Let's assume your new file is called `settings2.xml`. Add `[video-player-fx settings="settings2.xml"][/video-player-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `videoplayerfx_echo_embed_code()` function call (for example `<?php videoplayerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[video-player-fx]` and `[/video-player-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `videoplayerfx_echo_embed_code()` function call (for example `<?php videoplayerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[video-player-fx width="600" height="300"][/video-player-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `videoplayerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/video-player.html "Video Player FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/video-player-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/video-player.html "Video Player FX") is the utility that helps easily customize your Video Player FX to fit all your needs.