ApachePress
===========

ApachePress is a simple, WordPress-branded theme for your Apache directory listing.

##Installation

ApachePress requires an Apache(2.0.23+) enabled HTTP server.

Let's assume you have a folder named `share` in your server root directory (the path thus being `http://mywebsite.com/share`) that you'd like to use as your listing directory:

* Download and unzip ApachePress
* Copy and paste the contents of the `/apachepress` folder to your `/share` folder.
* Edit `htaccess.txt` (now in the `/share` folder) and update all instances of paths marked with *{FOLDERNAME}* to point to your site root.

So...

    AddIcon /{FOLDERNAME}/theme/icons/gif.png .gif

Should be changed to...

    AddIcon /share/theme/icons/gif.png .gif

* Once done, rename `htaccess.txt` to `.htaccess` in both the `/share` and `/share/theme` folders.