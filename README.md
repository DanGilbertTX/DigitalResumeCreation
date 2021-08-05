# Creating a Digital Resume

You will need several things to create a digital resume. In no particular order, you will need:

* Somewhere to host it. AWS or your own server are probably best. I went with a $6/mo. OVH VPS instance because I like headless Linux and know how to lock it down.
* A good template; I used iPortfolio from BootstrapMade: https://bootstrapmade.com/iportfolio-bootstrap-portfolio-websites-template/
* A text editor; I use Notepad++
* A background image you want to use; should be 1920x1080 for proper scaling
* Some personal pictures and your resume
* Time and patience



The end result will be something like this site (but hopefully much, MUCH better): https://burninggnome.net/

#### To start, download whatever template you want to your local computer and unzip it. Assuming you are using iPortfolio from the link above, the following files/directories are the ones you will be working with:

  * ./index.html
  * ./assets/img/
  * ./assets/css/style.css
  * ./forms/contact.php *`If you buy the template and want to use the contact form`*


Once you have the template unzip, go ahead and open ./index.html in both a web browers (so you can see changes) and in your text editor. Alternatively, you can steal my index.html page if you want. Just view source/view page source on that site and it will open up the index.html in the browser. Copy/paste it in to your text editor and start making changes there.

#### Other than content changes, here are specific items you will need to change (line numbers are the stock index.html) in the index.html file:

1. Line 8 - Change the title to something personal 
2. Lines 13 & 14 - Change the favicon (what shows up in the browser tab before the page title) to whatever you want. Regular is 32x32 and Apple Touch is 180x180
3. Line 48 - Insert your avatar picture here
4. Line 49 - Change the name
5. Lines 51 - 51 - These are links to social media or other sites. In the default they do not have a hyperlink. For your page you will need to add that like so: `<a href="https://github.com/DanGilbertTX" target="_blank" class="github"><i class="bx bxl-github"></i></a>`
6. Navbar starts at line 59. The href is the hotlink to each section. The ***i class*** is the icon show. iPortfolio comes with *boxicons* by default. If you want anything else you will need to add them on your own. I added fontawesome to my site for some of the icons later on. 
7. 


#### Background image in the Hero section (main background picture you see)

You will need to open the ./assets/css/style.css file. The **Hero Section** starts at line 211. The background itself is line 216. Download an appropriate picture and put it in the ./assets/img/ folder and then change the line in the style.css file.

As for what background to choose. That is up to you. There are a lot of free images on https://pixabay.com/. I searched for "*cloud computing*" on there and found some images I liked. Tested each one out to see how it looked. You will want to get a picture that is at least 1920x1080 so that it scales up or down well. A lower resolution picture will look really bad on a high resolution (49" ultra-wide for instance) monitor. 


## Helpful Links:
* https://boxicons.com/?query=
 * You can see what they look like and keyword search. It will give you the name of the icon and you may have to play around to get the syntax right in the html.
* https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free
 * Search here for for FA icons. 
* To use FontAwesome you will need to download the free package. The latest package is here: https://fontawesome.com/v5.15/how-to-use/on-the-web/setup/hosting-font-awesome-yourself
