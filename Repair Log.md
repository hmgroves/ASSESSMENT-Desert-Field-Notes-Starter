I1
Target and symptom: There was no language set for the site.
Cause: Lack of language declared at the start of the index html file.
Correction: Declared english language at the start.
Evidence: Nu html checker reported missing lang attribute.
Verification: Tested the code through Nu html checker both with and without lang attribute, with the attribute there was no warning and without there
    was a warning.

I2
Target and symptom: Missing meta viewport in head which affects how the CSS displays on mobile devices.
Cause: Missing element in head.
Correction: Added viewport meta to determine the width of the site via the width of the device viewing the site.
Evidence: https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/meta/name/viewport#viewport_width_and_screen_width 
Verification: Loaded the site on mobile and observed the differences with and without the viewport setting enabled. There is still some horizontal
    scrolling required (I assume from a CSS error) but the default size is much better with the viewport enabled.

I3
Target and symptom: Clicking on the 'Resources' link in the nav leads to a file not found error page.
Cause: In the navigation, the file being linked for the resources page is misspelled and doesn't account for the file being in a separate folder.
Correction: Corrected the spelling of the file name and added the folder path.
Evidence: Observed the error page in browser by interacting with the site.
Verification: Purposefully misspelled the file name again and got the same error.

I4
Target and symptom: The header hierarchy jumps from h1 to h3 making the text on the site for the intro smaller than it should be.
Cause: The header of the intro class is set to h3 instead of h2.
Correction: Changed the header to h2.
Evidence: Nu html checker reported an error of skipping a heading level.
Verification: Changed the intro class header to various incorrect heading levels and observed the different sizes on the site.

I5
Target and symptom: The alt text for the image doesn't properly describe the image's appearance or purpose.
Cause: Caused by the alt text for the image not being correct.
Correction: Changed the alt text to better reflect the image and its purpose.
Evidence: If the image is broken on the site, the insufficient alt text appears.
Verification: Breaking the image on purpose now shows the updated text.

R1
Target and symptom: The resources page doesn't load the style sheet and looks very plain.
Cause: The stylesheet reference didn't account for the css file being in a separate folder.
Correction: Added the correct file path.
Evidence: Observed the page not looking correct on the site.
Verification: If you change the referenced stylesheet, the page returns to not looking correct.

R2
Target and symptom: Clicking either the site title or the 'home' link on the resources page leads to a file not found error page.
Cause: The reference link for the site name and home button didn't account for proper folder paths.
Correction: Changed the pathing to be correct and link back to the main page 
Evidence: Observed the error page in browser by interacting with the site.
Verification: Changing these referenced links causes the error page to show again.

C1
Target and symptom: When using a keyboard to navigate you can't visually tell what link is currently selected.
Cause: Caused by a:focus in CSS setting the outline to none.
Correction: Deleted this setting.
Evidence: https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility/CSS_and_JavaScript#css
Verification: Reinstating this line of code has the outline vanish again.

C2
Target and symptom: The fixed width of the site-header, main, and footer causes horizontal scrolling on screens smaller than 1100px.
Cause: Width is set to 1100px for site-header, main, and footer.
Correction: I set the width to 90% so it dynamically scales with the screen size.
Evidence: Observed the content changing sizes depending on the window size.
Verification: Set the width to 100% and 80% to see how that affected the look as well.

C3
Target and symptom: The cards on the main page overflow the main section if the screen is too narrow.
Cause: A fixed card width of 300px causes this overflow.
Correction: Changed the card width to be 1fr and for the cards to stack in a column if the screen is less than 800px.
Evidence: The resulting look stays within the bounds of the main section and looks nicer.
Verification: Changed the width of the cards to various pixel sizes to see the results.

C4
Target and symptom: The orange color of 'featured card' overrides the green color of 'featured'
Cause: Caused by the 'featured card' having a higher weight in the CSS.
Correction: Added the 'where' exception to 'featured card' to allow the other style to take priority.
Evidence: https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Cascade/Specificity#the_where_exception 
Verification: Tried using this on headers as well to see if it had the same effect and it did.

C5
Target and symptom: The screen can never be less than 500px and more than 700px at the same time.
Cause: Caused by media query min and max conditions being impossible.
Correction: Changed maximum width from 500px to 700px and deleted minimum width so that the site looks nicer at scales under 500px.
Evidence: Observed smaller screen now has the nav and the cards wrap nicely to fit better.
Verification: Tried just swapping the numbers, but this only allowed the media condition for 200 pixels and the site looked odd at under 500px where the
    nav got squished back on the right and the card columns become hard to read.