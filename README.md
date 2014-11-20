ApachePress
===========

---

##About

ApachePress is a simple, WordPress-branded theme for your Apache directory listing.

---

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

---

##ApachePress themes

If you'd like to alter the default ApachePress theme, look in the `/theme` folder and you'll find the following files:

* `header.html`
* `footer.html`
* `style.css`

Edit these as you would any other HTML or CSS file.

Adding your own icons is a little more involved. You'll need to edit the main ApachePress `.htaccess` file. Look for the following as an example:

    AddIcon /{FOLDERNAME}/theme/icons/gif.png .gif

The above rule will assign an icon named `gif.png` from the directory `/{FOLDERNAME}/theme/icons/` to any file with the `.gif` extension.

This URL path is relative to your site's root.

---

##Mime Types

The default ApachePress theme `/theme` has icons in place for the following mime types:

    .aif .aif .asf .asx .avi .bin .c .css .csv .dmg .doc .docm .docx .dot .dotm .eps .flv .gif 
    .htm .html .ico .iff .jar .jpeg .jpg .js .json .log .m3u .m4a .md .mid .mov .mp3 .mp4 .mpa 
    .mpg .msg .mwa .odt .pages .pdf .pkg .png .ps .psd .ra .rar .rb .rm .rss .rtf .shtml 
    .sql .srt .swf .tex .tiff .txt .vob .wav .wmv .wpd .wps .xhtml .xlam .xlr .xls .xlsm .xlsx 
    .xltm .xltx .xml .zip