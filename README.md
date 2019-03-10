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
