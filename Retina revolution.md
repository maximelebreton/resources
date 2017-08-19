

[Source](https://www.netvlies.nl/tips-updates/algemeen/algemeen/retina-revolution/ "Permalink to Retina revolution - Netvlies")

# Retina revolution - Netvlies

**The devil is in the details**  
Detail is probably one of the most important values for a designer, an eye for detail should be in our DNA. As a perfectionist I like my designs to be pixel perfect. I am allergic for "jaggies" and ugly compressed artifacts in icons and images on websites. Apple's Retina revolution is an interesting evolution that is turning the design world upside down. The Retina display has a high enough pixel density to prevent pixelation to be noticable to the human eye. Therefore a Retina display is a lot sharper and more pleasant to look at. Apple has doubled the amount of horizontal and vertical pixels on the iPhone, The New iPad, and now also on the new MacBookPro. The Retina revolution is irreversible, and other companies have already started or will also start implementing this new Retina technology.

Nowadays pixel perfection can be obtained with techniques like @font-face and CSS3. Making fonts, borders, shadows, and gradients sparkle on your screen. These elements are based on vectors or mathematical expressions which allows them to be scaled to enormous sizes without creating distortion. This does not count for rasterized images which consist of pixels. An image that looks good on a normal display will appear blurry on a Retina display.  The Retina display blows up the image, it doubles the amount of pixels. There is not enough data for the image to be displayed properly.

So there really is only one solution to get these images to be displayed properly and that is to double the images in size. More pixels = better display! Plenty of articles have been written about this technique, like this article by [Conor Turnbull][1]. Turnbull's article shows how various companies like Apple are preparing their websites for the Retina revolution. In short: first the normal page will be loaded, then they detect if the page is viewed on a Retina display. If a Retina display is detected, images with a double pixel-size will be downloaded and will replace the normal images. This means that roughly 4 to 5 times more data will be downloaded compared to a normal website. Ridiculous right? Now that we finally have access to incredible Internet speeds we get thrown back in time. There doesn't seem to be a proper solution, and if so could this already be the end of the Retina revolution?

Thankfully not…

**More detail with less kilobytes**  
One thing is certain, if you want to solve this problem you will need bigger images. Images that are double in size. This has been the starting point in a few tests I have done.

I saved a 300 x 200 pixel image as an jpg image with an 80% compression, it's file-size was 21kb. This file, optimized for a normal screen resolution, formed the base for my test. I saved the same image, this time optimized for a Retina display, and doubled its size. So it had 4x the amount of pixels. With the exact same compression (80%) this image was 68kb. This makes sense of course, the image is 4 times as big. I then put the two images in a test HTML-page and scaled the Retina image 50% so that both images had the same format (300×200). When I opened the test HTML-page on the New iPad, with Retina display, the image was very sharp but unfortunately its filesize was just too big to actually start using this method.

I continued the test by saving the base image with 1,5 times the amount of kilobytes of the, doubled the pixel size, but with more compression than the first test. This image also appeared very sharp, but it's filesize was still far from ideal. So I continued to increase the compression of the image, and still the image appeared very sharp on a Retina display.

> A smaller filesize AND a better quality on both screen types! This is impossible.

"So why not continue compressing the Retina image" I thought to myself. I continued by reducing the Retina image to a whopping 75% of the base image. Holy moly, even this worked, even this image was razor sharp. The difference is even noticable on the iPad 1, 2 and normal computer screens. How bizar, the filesize is smaller than the original. So a smaller filesize AND a better quality on both screen types! This is impossible, I thought. I started to wonder if there was something wrong with the base-file that I used. But there was nothing wrong, I did various test with different images and they all had the same result. Eureka!

The bottomline is that heavy compression doesn't affect the final image as much as you would expect. This is because of the greater amount of pixels in the Retina image, compression artifacts are scaled down and therefore almost unnoticeable.

Of course there are certain factors that you have to consider before you start using this method in future websites. For example, how will these images behave in a responsive website? Also, is this something that clients can handle? How can the compression be determined, can a CMS automatically compress the images?

**Examples**  
In the left column you can see the base-images, in the right column the Retina images with various compressions. Make sure you check it on a Retina display of course!

[More examples can be viewed in the follow up article][2] (via Google Translate)

 

 

 

 

Translation by: Thomas Rademakers

[1]: http://webdesign.tutsplus.com/articles/general/improving-image-quality-on-the-retina-display/
[2]: http://translate.google.com/translate?sl=nl&tl=en&js=n&prev=_t&hl=en&ie=UTF-8&layout=2&eotf=1&u=http://blog.netvlies.nl/design-interactie/retina-revolutie-follow-up/&act=url "Retina revolution follow-up"

  
