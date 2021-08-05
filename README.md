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
2. Lines 13&14 - Change the favicon (what shows up in the browser tab before the page title) to whatever you want. Regular is 32x32 and Apple Touch is 180x180
3. Line 48 - Insert your avatar picture here
4. Line 49 - Change the name
5. Lines 51-55 - These are links to social media or other sites. In the default they do not have a hyperlink. For your page you will need to add that like so: `<a href="https://github.com/DanGilbertTX" target="_blank" class="github"><i class="bx bxl-github"></i></a>`
6. Navbar starts at line 59. The href is the hotlink to each section. The ***i class*** is the icon show. iPortfolio comes with *boxicons* by default. If you want anything else you will need to add them on your own. I added fontawesome to my site for some of the icons later on. 
  * NOTE: If you change a Navbar section name, make sure it matches up to the Section heading for the item later on in the index.html file.
7. Line 75 - Change the name
8. Line 76 - These are the adjectives that get typed out on the main (Hero) page. Change them to whatever you want. You can even change the *"I'm"* to something like *"Professional"* or *"Super Awesome Bad-ass doing"
9. Line 88 - Change this part of the About section to say something about yourself
10. Line 96-121 - Say more about yourself
11. Line 134-168 is the *"Facts"* section. I change it to *"Project Highlights"* and another changed it to *"Experience"*
12. Do the same for the ***Skills***, ***Resume***, ***Portfolio***, ***Services***, & ***Testimonials*** sections
13. Line 560 starts the ***Contact*** section. This includes a Google Map link that you will want to change.
14. Line 591 starts the Contact Form section. Please note that this will **NOT** work unless you buy the template. If you aren't buying the template then I would suggest removing the Contact Form.
15. Line 627 starts to Footer. Per the licensing terms you cannot remove this section unless you buy the template. If you do buy it, I would remove it. You do you though. 

* Bonus #1: ***IF*** you are adding custom icons (say FontAwesome for instance), you will need to add the link to the .css file for it in the *Vendor CSS Files* section starting at line 19. 
* Bonus #2: IF you want to add the flashing ***Download My Current Resume*** button you will need to add the code below (*Animate and style button*) to your style.css file in the at the bottom. Just paste in the code at the end of the file. 

#### Background image in the Hero section (main background picture you see)

You will need to open the ./assets/css/style.css file. The **Hero Section** starts at line 211. The background itself is line 216. Download an appropriate picture and put it in the ./assets/img/ folder and then change the line in the style.css file.

As for what background to choose. That is up to you. There are a lot of free images on https://pixabay.com/. I searched for "*cloud computing*" on there and found some images I liked. Tested each one out to see how it looked. You will want to get a picture that is at least 1920x1080 so that it scales up or down well. A lower resolution picture will look really bad on a high resolution (49" ultra-wide for instance) monitor. 


## Helpful Links:
* https://boxicons.com/?query=
  * You can see what they look like and keyword search. It will give you the name of the icon and you may have to play around to get the syntax right in the html.
* https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free
  * Search here for for FA icons. 
* To use FontAwesome you will need to download the free package. The latest package is here: https://fontawesome.com/v5.15/how-to-use/on-the-web/setup/hosting-font-awesome-yourself


### Animate and style button
`/* Animate and style button */
#resume > a {
  display: flex;
  margin: 0 12.5%;
  justify-content: center;
  align-items: center;
  border: none;
  height: 48px;
  box-shadow: 0 0 0 0 rgb(20 157 221);
 
  -webkit-animation: resume-pulse 2.25s infinite cubic-bezier(0.54, 0, 0, 1);
  -moz-animation: resume-pulse 2.25s infinite cubic-bezier(0.54, 0, 0, 1);
  -ms-animation: resume-pulse 2.25s infinite cubic-bezier(0.54, 0, 0, 1);
  animation: resume-pulse 2.25s infinite cubic-bezier(0.54, 0, 0, 1);
}
 
#resume > a > i {
  padding: 0 12px;
}
 
/* Dont animate when mouse is on button */
#resume > a:hover {
  -webkit-animation: none;
  -moz-animation: none;
  -ms-animation: none;
  animation: none;
}
 
@-webkit-keyframes resume-pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
@-moz-keyframes resume-pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
@-ms-keyframes resume-pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
@keyframes resume-pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}`
