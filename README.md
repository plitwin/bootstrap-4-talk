# Bootstrap 4 Talk - Building a website with Bootstrap 4
#### https://www.meetup.com/Seattle-Web-App-Developers-Group/events/259308386/
#### Paul Litwin

# Folders and Files
* Major steps use letters as in Step A, Step B, etc.
* The final version of each step will be in that Steps folder.
* The artist artwork appears in ACE_Website.pdf.
* Additional html/css that is to be copied into steps can be found in BS 4 Talk Clipboard.txt.

# The Steps

## Step A
1. Mkdir dirname
4. Start terminal
5. dotnet new mvc
6. Open VS Code
7. Run starter app usig dotnet run
---
8. Open wwwroot\lib\boostrap\dist folder and delete contents
9. Copy dist folder from downloaded bootstrap here
10. Refresh browser to see how bad it looks
 * Note diferences between Bootstrap 3 and Bootstrap 4
---
10. Copy Bootstrap 4 starter template from 
    https://getbootstrap.com/docs/4.3/getting-started/introduction/
    and paste into Views\Shared\_layout.cshtml page
11. Refresh browser
 * whoops - no @RenderBody() section
---
13. Add @RenderBody() just under <body> 
14. Add @RenderSection("Scripts", required: false) just above </body>
15. Preview.
---

## Step B
1. Hmmm. How about getting the layout and site.css from here instead: https://medium.com/@ashwinigupta/how-to-migrate-from-bootstrap-3-template-to-4-in-asp-net-core-application-7da01a1acf99
17. Remove site.css.min
18. Preview.
19. I like the footer but let's ditch the navbar for now since it's not quite what we want.
10. Change color in site.css fro footer to background-color:#48D8C1;
11. Add  text-center to div tag
12. Add text-white to span and add text "&copy Fred Hutchinson Cancer Research Center @DateTime.Now.Year. All rights reserved."
13. Preview.
---
14. Okay. Time to remove content from Index page and start over.

## Step C
1. Remove everything from Index page except for title and some placeholder text.
2. Let's look at the art work. 
3. Not sure I like the Nav Bar. Let's do something similar but better.
4. Copy Navbar text in (Version 1) for Layout page from BS Talk Clipboard.
 * Note that there is no indication of which page is current. But you could set the active page 
from the layout by querying the title of the current page and specifying the active class conditionally based on the value of title in the ViewBag.
6. Copy final version Navbar.
7. Preview
7. Back to Index. 
 * Note complexity of art work for top of page with image of women at bar plus overlaid script image, text, and button. Cards allow us to easily create these overlays.
using the card-img-overlay class.
7. Copy in Version 1 of Top of page.
 * Note what happens and site goes down in size to landscape phone mode (sm) and then to portrait mode (xs). Doesn't look very good.
* Note the "d" classes. They let you decide when (at what breapoint) an element will be shown.
    *  d-none means don't display starting at xs size
    * d-md-block means display starting at md size
    *  d-sm-block means display starting at sm size
7. Preview
8. Now copy final version of Top of page and show how it looks.
8. Preview.
9. Now to bottom of page.
10. Copy Bottom of Page text in to page. Noteworthy items include...
 * p* and m* which sets padding and margin, respectively. Where * can be...
    * (empty)= all sides,
    * t=top, 
    * b=bottom, 
    * l=left, 
    * r=right. 
    * x=left and right,
    * y=top and bottom.
 * using a font-awesome font for the downward arrow on the left side.
10. Preview.
11. We are still missing some coloring of things. 
12. Copy in additional classes to Layout file.
13. Preview. 
