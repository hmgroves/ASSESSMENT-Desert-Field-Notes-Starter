The error I selected for my code defense is the error with the ID I3. 

This error made it so that when you clicked on the 'Resources' link in the navigation section of the home page, it lead to a file not found error page.

This was caused by a line of code in the nav-list class in the index.html file. The code linking the resources.html file to the appropriate nav link had the source file both misspelled and didn't have the proper folder paths listed as the resources.html is in a separate folder.

This was corrected by spelling the resources.html file name correctly and linking to it via it's folder path ("pages/resources.html"). The instructions for how to correctly do so can be found here: https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Creating_links#moving_down_into_subdirectories 

After this correction, clicking on the 'Resources' link in the navigation section of the home page leads to the proper resources page,