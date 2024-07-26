Dave Gray YouTube tutorial for Tailwind CCS to create an Acme Rockets website completed 26/07/2024 (https://www.youtube.com/watch?v=lCxcTsOHrjo&t=7441s)

Learnt how to set up Tailwind and use it. 

Some notable comments / content from the tutorial:

Created a custom media query by extending (ie not overwriting) the Tailwind code in the tailwind.config.js file with a wide and tallscreen scenarios as well as a custom section-min-height calculated value in the style.css file using @layer utilities. We applied tall and widescreen:section-min-height classes to the three section elements of the html to ensure the full header was always visible when navigating 

We used @apply in the style.css file to create a custom class (not recomended for normal css style for reasons listed on the tailwind website). In this case it was used for a javascript controlled animation. Using the & symbol we created a pseudo selector for >div. In normal css our case would have been hamburger-button>div but in this case the javascript toggles a new class name "toggle-button" onto the element and activates / disactivates the toggle-button>div selector 


arbitrary values can be acheived using square brackets (eg for the top of the #mobile menu top-[68px] because 68px was not available as one of the standard options)

prettier (which i didnt use) orders classes for improved collaboration (colleagues always see the classes in the standardised order)

interesting code for: 
including email and phone numbers with href attributes to automate emailing or phoning someone (see footer)
scroll margin (to stop nav bar links hiding the title of the section: scroll-mt-20 (Aka scroll-margin-top:))
dark mode media query
Tailwind allows you to apply media queries easily. For example screen sizes: 
sm: 480px
md: 768px
lg: 976px
xl: 1440px

interesting link for emojis: https://emojipedia.org/
interesting link for symbols: https://symbl.cc/en/

Potential improvement - improve the javascript so that the toggle-button only displays the X when the menu screen is showing (and never when the full webpage is showing)