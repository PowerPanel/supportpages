# CSS example control panel

You can change every bit of our Control Panel with your custom css. Just look up the CSS selector and change it to your own style.
Reminder: the changes are visible after you log off and on again. This is because you need to renew your session to load the new CSS.

The location where you add your CSS is Settings -> Branding -> CP branding

This is the custom CSS we used to create our login page:

```css
div#login_box a {color: #339999;}
.masthead-title, div.header, h1, h2, h3, h4 {color: #0086BF}
legend {color: #339999; font-weight: bold;}
div#menu ul li a.active {color: #339999;}
div#submenu ul li a.active {color: #0086BF;}
div.paginatie a {color: #44B9EA;}
div#content_left ul li a.active {color: #0086BF;}
div#content_left ul li ul li a.active {color: #0086BF;}
div.input_row .blue {background: #009FE2;}
a.navbar-brand img {width:52px}
.navbar-text {color:#fff;}
ul.nav.navbar-nav.navbar-right li a {color:#000 !important;}
```

Here is a color example for your control panel :

https://cp.powerpanel.io/includes/css/colors.css


# CSS example Webshop

You can change every bit of our Control Panel with your custom css. Just look up the CSS selector and change it to your own style.
Reminder: the changes are visible after you log off and on again. This is because you need to renew your session to load the new CSS.

The location where you add your CSS is Settings -> Branding -> Webshop branding

This is the custom CSS we used to create our webshop:

```css
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
```
Here is a color example :

https://demoshop.mypp.io/includes/css/colors.css