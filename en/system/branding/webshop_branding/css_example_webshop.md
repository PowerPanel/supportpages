# CSS example Webshop

You can change every bit of our Control Panel with your custom css. Just look up the CSS selector and change it to your own style.
Reminder: the changes are visible after you log off and on again. This is because you need to renew your session to load the new CSS.

The location where you add your CSS is Settings -> Branding -> Webshop branding

This is the custom CSS we used to create our webshop:

/*** header ***/
#navigation { background-color: #1982E3; }
#navigation .icon { background-color: #1982E3; }
#navigation .icon:hover,
#navigation .login:hover .icon { background-color: #a46cbb; }
#navigation .icon:active,
#navigation .login:active .icon { background-color: #855898; }
#navigation ul.menu {background-color: #2B1038;}

/*** timeline ***/
#timeline .logo a img {width: 191px;height: 48px;}
body.scrolled #timeline .logo a img { width: 165px; height: 41px;}
#timeline .bar .filled { background-color: #1982E3; }
#timeline .nodes li.active .circle { border-color: #1982E3; }
#timeline .nodes li.active .label,
#timeline .nodes li.done .label { color: #1982E3; }
#timeline .nodes li.done .circle { background: #1982E3; }
#timeline .nodes .steps span.sub-active { color: #1982E3; }

Here is a color example :

https://demoshop.mypp.io/includes/css/colors.css
