favicon
=======

HTML5 Favicon Generator
-----------------------

- Generates 'perfectly' resampled icons with sizes 192x192, 144x144, 96x96, 64x64, 48x48, 32x32 and 16x16 from a single 576x576 image.

- It creates a PNG for each size and generates Windows ICO file from selected image sizes.

Now, what I mean by 'perfectly':

- It edits the images in linear RGB space, so that it doesn't make the common mistake of doing color math in sRGB space which doesn't matter much in a megapixel photo with smooth color transitions but matters in a 16x16 icon with sharp color changes. (BTW: even Adobe Photoshop gets this wrong).

- It uses 32 bit floating point per channel, so that it doesn't lose bit depth, which -again- Adobe Photoshop loses if you don't manually change bit depth to 16 bits per channel before you do anything to your image. Most users don't (know how to or why they should) do that.

- Bonus: It also creates RGB subpixel-antialiased versions of each icon, so you can fully utilize that small 16x16 space you're given.

Also this project was a rehearsal for a sophisticated HTML5 image editor.
