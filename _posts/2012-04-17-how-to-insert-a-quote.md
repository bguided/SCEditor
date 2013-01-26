---
layout: post
title: How to insert quotes
excerpt: Breif example of how to insert a quote
tags: [HTML, BBCode, demo, example]
categories:
    - Demo
    - BBCode
    - HTML
---
## Quote demo

<script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"> </script>
<link rel="stylesheet" href="/minified/themes/default.min.css" type="text/css" media="all" />
<script type="text/javascript" src="/minified/jquery.sceditor.bbcode.min.js"> </script>
<script>$(document).ready(function() {
	$("#demo-quote").sceditor({
		plugins: 'bbcode',
		style: "/minified/jquery.sceditor.default.min.css",
		emoticons: {
			dropdown: {
				":)": "/emoticons/smile.png",
				":angel:": "/emoticons/angel.png",
				":angry:": "/emoticons/angry.png",
				"8-)": "/emoticons/cool.png",
				":'(": "/emoticons/cwy.png",
				":ermm:": "/emoticons/ermm.png",
				":D": "/emoticons/grin.png",
				"<3": "/emoticons/heart.png",
				":(": "/emoticons/sad.png",
				":O": "/emoticons/shocked.png",
				":P": "/emoticons/tongue.png",
				";)": "/emoticons/wink.png"
			},
			more: {
				":alien:": "/emoticons/alien.png",
				":blink:": "/emoticons/blink.png",
				":blush:": "/emoticons/blush.png",
				":cheerful:": "/emoticons/cheerful.png",
				":devil:": "/emoticons/devil.png",
				":dizzy:": "/emoticons/dizzy.png",
				":getlost:": "/emoticons/getlost.png",
				":happy:": "/emoticons/happy.png",
				":kissing:": "/emoticons/kissing.png",
				":ninja:": "/emoticons/ninja.png",
				":pinch:": "/emoticons/pinch.png",
				":pouty:": "/emoticons/pouty.png",
				":sick:": "/emoticons/sick.png",
				":sideways:": "/emoticons/sideways.png",
				":silly:": "/emoticons/silly.png",
				":sleeping:": "/emoticons/sleeping.png",
				":unsure:": "/emoticons/unsure.png",
				":woot:": "/emoticons/w00t.png",
				":wassat:": "/emoticons/wassat.png"
			},
			hidden: {
				":whistling:": "/emoticons/whistling.png",
				":love:": "/emoticons/wub.png"
			}
		}
	});
});

function insertQuote(includeAuthor)
{
	// first get the editor's instance
	var editor = $("#demo-quote").sceditor("instance");

	// execute the insert command
	if(includeAuthor)
		editor.insert('[quote=author]This is an [b]example[/b] quote.[/quote]');
	else
		editor.insert('[quote]This is an [b]example[/b] quote.[/quote]');
}

</script>

<textarea style="width:600px; height:300px" id="demo-quote">This [b]is[/b] [color=#ff0000]a[/color] [size=3]demo[/size] :).</textarea>
<a href="javascript:insertQuote();">Insert Quote</a> | <a href="javascript:insertQuote(true);">Insert Quote with author</a>

## Code behind it

To insert a quote, just pass the quotes BBCode to the `insert()` command.
e.g.:

{% highlight javascript %}
// first get the editor's instance
var editor = $("#demo-quote").sceditor("instance");

// execute the insert command
editor.insert('[quote=author]This is an [b]example[/b] quote.[/quote]');
{% endhighlight %}

