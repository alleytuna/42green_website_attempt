# 42green_website_attempt

some guidelines
- choose a green webhost (regulated tech waste management, green data centers or CDN datacenter located near users - edge computing, social inclusion taken into account, renewable energies, low carbon) or a Raspberry Pi (sounds good for static website)
    to explore: aiso.net, hostgator, GreenGeeks, A2 Hosting, iPage, HostPapa, Acorn Host
- opt for a static website when possible (reduce redirections)
- using fewer JS widgets or none, reducing image/video, focus on a quick loading (test site speed / caching solutions)
- create a responsive website (format adapted to each device: smartphone, desktop computer, tablet)
- website icon: put the favicon.ico (icon next to the website name) in cache
- basically, compress anything compressable (images, HTML code, CSS, JS lib, PDF, any files ==> abuse of gzip,brotil, zopfli)

Structure
- check that HMTL is valid with W3C otherwise it'll be done automatically each time used
- use a linter (like YUI compressor) to delete useless elements of any code
- combine CSS and JS files

Images
- use glyphs sprites and pseudo elemens instead of images
- optimise vector graphics and CSS effects with small files such as JPEG and GIF
- upload image at scale instead of relying on CSS auto resizing (not necesseray on WordPress as its uspport responsive images)
- compress (SVGO)

Server
- use a asynchronous server (do not create a new process or thread for a new request)
- compress HTML to limit bandwith between host and server
- use ETags

Caching optimisation/level
- Caching systems must be mounted in RAM if possible
- Bytecode cache for auto compilation
- Object cache to store database queries' results
- Page cache stores the entire HTML of a page (have a look at [nginx fastcgi cache module]; possibility to modify the cache expiration)
- CDN cache stores website files (JS, CSS, media files) = reduces server resources required to load a site 
- caching 404 pages, or even create only one common 404 page for error redirection



An amazing checklist to follow: https://collectif.greenit.fr/ecoconception-web/2019-05-Ref-eco_web-checklist.v3.EN.pdf (FR version available as well)