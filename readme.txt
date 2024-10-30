=== Image Zoomer FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, image, zoomer, effect, free, flash, as3, xml, animation, movement, customizable, autoscroll, transition, dragscroll
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced Image Zoomer on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It supports images (JPG, BMP, PNG, GIF) and SWFs with customizable widths and heights for the whole application. It has auto scroll functionality with customizable controls or navigation window for zoom in/out and movement directions. There are many other particular properties available on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/image-zoomer-fx.zip "Image Zoomer FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/image-zoomer.zip "Image Zoomer FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **image-zoomer-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Image Zoomer FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[image-zoomer-fx][/image-zoomer-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Image Zoomer FX part of your theme, edit the template files and add `<?php imagezoomerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Image Zoomer FX](http://www.flashxml.net/image-zoomer.html "Image Zoomer FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/image-zoomer-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/image-zoomer-fx/images/` and update the `wp-content/flashxml/image-zoomer-fx/images.xml` file accordingly

= Additional settings file =

To embed the Image Zoomer FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[image-zoomer-fx settings="settings2.xml"][/image-zoomer-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `imagezoomerfx_echo_embed_code()` function call (for example `<?php imagezoomerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[image-zoomer-fx]` and `[/image-zoomer-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `imagezoomerfx_echo_embed_code()` function call (for example `<?php imagezoomerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[image-zoomer-fx width="600" height="300"][/image-zoomer-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `imagezoomerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/image-zoomer.html "Image Zoomer FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/image-zoomer-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/image-zoomer.html "Image Zoomer FX") is the utility that helps easily customize your Image Zoomer FX to fit all your needs.