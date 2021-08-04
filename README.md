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

#### Other than content changes, here are specific items you will need to change (line numbers are the stock index.html):

1. Line 8 - Change the title to something personal 
2. Lines 13 & 14 - Change the favicon (what shows up in the browser tab before the page title) to whatever you want. Regular is 32x32 and Apple Touch is 180x180
3. Line 48 - Insert your avatar picture here
4. Line 49 - Change the name
5. Lines 51 - 51 - These are links to social media or other sites. In the default they do not have a hyperlink. For your page you will need to add that like so: `<a href="https://github.com/DanGilbertTX" target="_blank" class="github"><i class="bx bxl-github"></i></a>`
6. 
