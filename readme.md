Important tips you can use on any website:

    - Use a CSS reset stylesheet.
        - When you do this, it resets the styling of all properties!
            This means things like h1's, h2's, links, lists, buttons. EVERYTHING will look the same.
            The font size, weight, borders, background colors will all be exactly the same and will display nothing fancy.
            So you need to create a root styling for all of these.
    - Have a main.css stylesheet which can be shared across all the pages of the website.
        - What you will do with this is essentially control the overall styling defaults.
          Like the h1,h2, lists, links, buttons styling for the whole page from here.
          You will also create the styling for the header and footer here, as you can then use these across the pages.
    - Create a {insert page name}.css style sheet to control those elements of the content other than the header and footer here.
        - we can can then style those elements independently to the header and footer.
    - The :root and html tag in the main.css file creates a root styling which will then be applied to all the other style sheets.
        - In the reset.css style sheet the default font becomes 16px, then inside of the actual root set the font size to 62.5%,
          this then makes the font size 10px.
        - This allows the rem font measurement to be easy to use as it is 1.6 * 10px = 16px.
        - When you use rem you can use unit-less line height. Google the rule of thumb measurements for the line height based on what value rem you used.
          e.g. default font = 16px
               In the root you set font-size to 62.5%
               Font now becomes 10px
               set font size in elements to 1.6rem which equals 16px
               then line height rule of thumb is 1.75
        - You can also use rem to scale height and width for box sizing, if there is text in the box.
    -Create the wrapper-main div class and then put the rest of your content into there.
        - It creates the overall alignment for your website.
        - You then just need to add the css styling in the main.css file once.
    - For mobile devices:
        - The wrapper main should not have a fixed with instead set it to 100%
        - You then set a new CSS styling property where you can dynamically swap things around:
            - You have to create a media query.
            - You have to have the meta tag in the html file with the viewport.
            - You must have wrapper-main div in your HTML and CSS main
            - The below is assuming you started working on desktop first then worked on mobile optimization.
            - The "only screen and" portion is a safety setting to have.
            - @media only screen and (max-width: 600px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 601px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 768px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 992px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 1200px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }
            All of the above are the major break points, just see if you have a 1000px then you dont need to add the 1200px. 
            These above are rule of thumbs.

            The below can also be set if the user switches to landscape mode and you can style based on portrait also seperately.

            @media only screen and (max-width: 600px) and (orientation: landscape){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

            @media only screen and (max-width: 600px) and (orientation: portrait){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 601px) and (orientation: landscape){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 768px) and (orientation: landscape){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 992px) and (orientation: landscape){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 1200px) and (orientation: landscape){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }
            
            You could remove all of those and write it simply like. you must have the first max width.

              @media only screen and (max-width: 600px){
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }

              @media only screen and (min-width: 601) and (max-width: 768) {
                .wrapper-main {
                        width: 100%;
                        
                        }

                 }
        
        - You can actually choose to remove content based on the mobile device.


----------------------------------------------------

2025/02/25

This is going to be a build of my first portfolio website.
I will be starting with creating the nav bar and styling it using CSS basics.

    - Some concepts I will be applying here will be the use of flex-box and some image transitions.
    - I intend to have some social media links in the nav bar along with an AI generated image of a company logo that I designed.
    - the use of the VAR function in HTML.
    - Pre loading images into the file to make the transition a bit smoother.
    - Use of CSS reset file on all pages.
    - Application of adding a custom font to the webpage.

I will also be adding the other webpages that the menu will look at and then use that nav bar style for the CSS of those websites.

This will be almost a journal and description of what I am learning and how I am going to also keep track other than git on what I have done to the website.

I will update this as I make big changes to the webpage.

I will be adding comments to some places in the code so I can reference back to what I have done there so the code might be a bit bloated.

---------------------------------------------------

2025/02/25 10:53am

The nav bar is now complete. I have added a lot of comments to the code so that I can refer back to certain sections for future reference.

I have structured it in such a way that I can use this for basic and generic websites in the future.

The nav bar actually has icons which link to my different social media platforms for professionals and is black and white and once you hover over it, it actually changes to color.

--------------------------------------------------------

2025/02/25 11:30am

Started work on the hero portion of the webpage.

Added some more default styling to the header.css file as the rest seems to have reset all the 
default styling on the webpage.

I then added some background images.

I learnt that the calc function can be used to help with calculating where things should be.

-------------------------------------------------------------

2025/02/25 16:03pm

After working on the hero section, I took it upon my self to add a log menu and page.
The purpose of this is to actually put this on the website and keep it up to do date with this file.
That took a bit of time and I created only the hero section of but haven't actually filled out any of the content there.

The Category section is now complete, I learnt a few new techniques for a dark hover effect.

I followed a tutorial and think I have a bit of a better way to actually design this, it is a little bit more cumbersome but works slightly better.

I played around a bit with the borders and also adding a gif as a hover effect which is pretty cool.

Next up is creating the about me section on the main page.

Just take into account there is a lot of filler information for the time being, like placeholder images and text.

------------------------------------------------------------------

2025/02/25 17:05pm

Completed the about section.

Only cool thing of note here was creating "skill bars"

---------------------------------------------------------------------

2025/02/25 21:56pm

Finished the footer and sitemap of the website.

-----------------------------------------------------------------------

2025/02/26 09:54am

Shifted the website away from px for font size and moved over to REM measurement and unit-less line height.