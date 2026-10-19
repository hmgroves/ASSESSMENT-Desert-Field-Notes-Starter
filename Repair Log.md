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
Verification: What test did you repeat, and what happened?

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
Target and symptom: What failed or was inappropriate?
Cause: Which markup, path, selector, declaration, or condition caused it?
Correction: What did you change?
Evidence: Which MDN page, browser observation, or validator result supports the decision?
Verification: What test did you repeat, and what happened?

C3
Target and symptom: What failed or was inappropriate?
Cause: Which markup, path, selector, declaration, or condition caused it?
Correction: What did you change?
Evidence: Which MDN page, browser observation, or validator result supports the decision?
Verification: What test did you repeat, and what happened?

C4
Target and symptom: What failed or was inappropriate?
Cause: Which markup, path, selector, declaration, or condition caused it?
Correction: What did you change?
Evidence: Which MDN page, browser observation, or validator result supports the decision?
Verification: What test did you repeat, and what happened?

C5
Target and symptom: What failed or was inappropriate?
Cause: Which markup, path, selector, declaration, or condition caused it?
Correction: What did you change?
Evidence: Which MDN page, browser observation, or validator result supports the decision?
Verification: What test did you repeat, and what happened?