---
layout: base
title: What I learned in a Programming Logic and Design Course
published: true
excerpt: If your going to introduce more advanced programming techniques into your code, use them correctly.
categories: blog
---

##{{ page.title }}

First off this is a 101 class. I consider myself "experienced" in programing JS. But I realized, coding for a "job" or for pleasure is much different than coding for a class.
Here's what happened
{% highlight javascript %}

function calculate_cone()
	{
	 "use strict";
// initialize names of variables
	var height, PI = 3.14159, radius, voloutput, message, radius;

// give each variable a value
	radius		= document.getElementById('radiusinput').value;
	height		= parseFloat(document.getElementById('heightinput').value);
// I ended up using math.round due to wayyy to many trailing numbers
	voloutput	= Math.round((PI * Math.pow(radius, 2) * height)/3);

// the massage the user will see after user clicks button
	message		= 'the volume is ' + voloutput;

	document.getElementById('volcone').innerHTML = message;
	}
{% endhighlight %}

Embarrassing code.

###Here
I did this to make myself feel a little better. No conditionals.
{% highlight javascript %}
function Calc(myform)
 {
  var base 	= document.myform.baseinput.value;
  var height	= document.myform.heightinput.value;
  var base 	= Math.pow(base,2);
  document.myform.volume.value = 1/3*base*height*Math.PI;  
	
 }
{% endhighlight %}

###Conclusion
1.	Don't code intro-style and throw in advanced techniques here-and-there, just because it's an intro level course doesn't mean you can code shit and get away with it. My code AND the outcome are both graded. I ended up with a 85% when I could've easily gotten a 100%.

2.	Spend time on your code and be proud if it. always question, always test.

Anyway no more playing around, this is an easy class. I've got to focus, keep an open mind, and put as much time/effort into school-coding as I do at home.