# 42green_website_attempt

some guidelines
- choose a low carbon webhost (to explore: GreenGeeks, A2 Hosting, iPage, HostPapa, Acorn Host)
- using fewer JS widgets or none, reducing image/video, focus on a quick loading (test site speed / caching solutions)

Images
- optimise vector graphics and CSS effects with small files such as JPEG and GIF
- upload image at scale instead of relying on CSS auto resizing (not necesseray on WordPress as its uspport responsive images)
- compress

Caching optimisation
- Bytecode cache for auto compilation
- Object cache to store database queries' results
- Page cache stores the entire HTML of a page (have a look at [nginx fastcgi cache module]; possibility to modify the cache expiration)
- CDN cache stores website files (JS, CSS, media files) = reduces server resources required to load a site 
- caching 404 pages