cf7-country-state-list
======================

Contact Form 7 - Country / State List.

I had issues with adding a dynamic list of countries / states to Contact Form 7.  
Luckly I found this script and incorporated it into Contact Form 7 for Wordpress.
**It's a standalone Country + State Javascript combobox/dropdown. You do not need Wordpress for this to work.**
Feel free to add improvements to the code. 


[Original article](http://bdhacker.wordpress.com/2009/11/21/adding-dropdown-country-state-list-dynamically-into-your-html-form-by-javascript/)

[Updated default selection article](http://jansouza.com/2010/10/13/javascript-country-state-list/)


Wordpress installation
======================
Example:
Here we are using twentyeleven as the theme of choice.

Please place the file accordingly, depending on whatever theme you are using.

1. Copy countries.js to:
/wp-content/themes/twentyeleven/js/countries.js


2. Open header.php:
/wp-content/themes/twentyeleven/header.php


3. Add this to your header file before `` </head> ``:
```
<script type= "text/javascript" src = "<?php bloginfo('template_directory'); ?>/js/countries.js"></script>
```
---

Now make a new form in Contact Form 7.
Add:
```
	Country:
		<select onchange="print_state('state',this.selectedIndex);" id="country" name = "country"></select>
	State:
		<select name ="state" id = "state"></select>
		<script language="javascript"> print_country("country","USA");</script>

```
If you notice USA is the default country, this can be changed to your liking.

*So how do you include what was selected in the Message body?*

It's as simple as:

Country:
[country]
State:
[state]

------

[Contact Form 7](http://wordpress.org/extend/plugins/contact-form-7/)

[Questions for Contact Form 7](http://wordpress.org/support/plugin/contact-form-7)
