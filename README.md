# bootstrap-4-talk
Building a website with Bootstrap 4

# Steps
1. Install Dotnet core
2. Install VS Code
---
3. Mkdir dirname
    4. Start terminal
    5. dotnet new mvc
6. Open VS Code
7. Run starter app usig dotnet run
---
8. Open wwwroot\lib\boostrap\dist folder and delete contents
9. Copy dist folder from downloaded bootstrap here
10. Refresh browser to see how bad it looks
12. Discuss diferences between Bootstrap 3 and Bootstrap 4
---
10. Copy Bootstrap 4 starter template from 
    https://getbootstrap.com/docs/4.3/getting-started/introduction/
    and paste into Views\Shared\_layout.cshtml page
11. Refresh browser
12. whoops - no @RenderBody() section
---
13. Add @RenderBody() just under <body> 
14. Add @RenderSection("Scripts", required: false) just above </body>
15. Preview.
---
16. Hmmm. How about the layout and site.css from here: https://medium.com/@ashwinigupta/how-to-migrate-from-bootstrap-3-template-to-4-in-asp-net-core-application-7da01a1acf99
17. Remove site.css.min
18. Preview.
19. I like the footer but let's ditch the rest of the navbar for now. 
10. Change color in site.css to background-color:#48D8C1;
11. Add  text-center to div tag
12. Add text-white to span and add text "&copy Fred Hutchinson Cancer Research Center @DateTime.Now.Year. All rights reserved."
13. Preview.
---
14. Okay. Time to remove content from Index page and start over.

