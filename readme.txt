=== Genericon'd ===
Contributors: Ipstenu
Tags: icons, genericons, font icon, UI
Requires at least: 3.5
Tested up to: 3.6
Stable tag: 1.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Enables easy use of the Genericons icon font set from within WordPress.  Icons can be inserted using either HTML or a shortcode.

== Description ==

Genericons are vector icons embedded in a webfont designed to be clean and simple keeping with a generic aesthetic.

A full list of the Genericons icons is available: [http://genericons.com/](http://genericons.com/)

To use any of the Genericons icons on your WordPress site you can use basic HTML (for inserting in themes and functions) or shortcodes (for use in posts or widgets). You can adjust the size of the icons via css or, when using the shortcode, the size attribute. Default size is 16px.

To display the Twitter icon:

HTML: `<div class="genericon genericon-twitter"></div>` or `<i class="genericon genericon-twitter"></i>`

Shortcode: `[genericon icon=twitter]` or `[genericon icon=twitter size=32]`

== Installation ==

Install as a normal WordPress Plugin

Add shortcode or HTML to your posts, pages and even widgets to display a Genericons icon.

== Frequently Asked Questions ==

= Aren't they called Genericons with an S? =

Yes, but Genericon'd is a Zaboo-esque sort of way of saying 'These icons have been genericonified!' I was in a The Guild frame of mind. Also since this is not the official plugin, I didn't want to use that slug.

= What are all the codes to use? =

If you're like me, you forget this alllll the time. On your WP dashboard, go to Apperance -> Genericon'd. The page there will show you everything you need to know about using Genericons.

= Can I add it to menus? =

Yes! If you use CSS classes, you can apply a class like this:  `genericon genericon-facebook` You may need to jigger about with css to make the layout perfect.

= How do I change colors? =

The power of CSS! If you want to change the color to red for all genericons, add `.genericon {color:red;}` to your theme's CSS. If you just want Twitter to be blue, add `.genericon-twitter {color:blue;}` and so on and so forth. Colors are based on font, you see.

= Okay, but I want to change color in just this one use... =

I know what you mean. Try this: `[genericon icon=twitter color=blue]`

It uses inline styling, which I hate, but this was the best way to solve the problem that I could find (suggestions welcome).

= Speaking of, can I make just this one icon bigger? =

Sure can! Use this: `[genericon icon=twitter size=2x]`

You can use 2x through 6x. Anything else punts it to 1x.

= How about changing the hover-color? =

While I certainly could write that in, I decided not to. You certainly can do this with CSS, however I feel you should only be changing color when there's an action, like hovering over a link, and generally you've already done that. But if you want to manually do it in your CSS, it would go like this: `.genericon-twitter:hover {background-color:pink;color:purple;}`

= Why don't these work on IE 7? =

Genericons itself <strong>does not come with fallback icons by default</strong> -- therefore you have to create them yourself. If you are using HTML similar to this example: <code>&lt;span class="genericon genericon-warning"&gt;&lt;/span&gt;</code>

You can use the asterisk hack to serve a different icon to IE7 once you have saved the fallback icons to your project:

<pre>.genericon-warning {
    *background: url(fallback-icon.png) no-repeat center center;
    *text-indent: 100%;
}
</pre>

== Screenshots ==

1. Genericon'd help page
2. Zaboo, patron avatar of Genericon'd

== Changelog ==

= 1.2 =
* 2013-03-07
* Added in variable for size to allow for on-the-fly adjustments to color and size.
* Changed image size from 16px to 1em (this isn't perfect, but allows for smexier resizing)
* Fixed broken settings pages.

= 1.1 =
* 2013-03-06
* Tweaks and adjustments. 
* New banner (thanks to Joen)

= 1.0 =
* 2013-02-27
* Initial release