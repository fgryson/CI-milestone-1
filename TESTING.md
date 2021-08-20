# Testing

## Code validators

[HTML Validator](https://validator.w3.org/) : 

All pages passed without errors and only one warning that was shared between all pages as it was in the shared Contact pane.

![HTML validation warning](readme-images/html-validation-warning.png)

I decided to leave this warning as it was part of the embedded twitter element and was the HTML code provided by their documentation.

[CSS Validator](https://jigsaw.w3.org/css-validator/) : 

![CSS validation error](readme-images/css-validation-error.png)

CSS validation threw one consistent error, all the result of the method I used to apply alpha transparency to colour variables. The colour had to be stored as a CSS variable which contained three seperate value (Red, Green, and Blue) which would be passed into an RGB or RGBA css function as required. While visually this has the desired effect the validator throws an error.

## Responsiveness

Using both the Chrome and Firefox development tools I tested the project for responsiveness. I also tested the project physically on mobile througout development using the Live Server extension for VSCode.

![AmIResponsive image](readme-images/amiresponsive.png)

![Screenshot of website on mobile](readme-images/mobile-screenshot.jpg)

## Browser compatibility

Browsers tested:
- Firefox
- Chrome
- Edge
- Edge on Android

Having tested the project on these browsers I found no issues with responsiveness or appearance.

## Testing User stories

- As the academic, I want to introduce myself to the user.
  - When the user enters the site the are greeted by a portrait of the academic and also an introductory paragraph that highlights her main achievements on the **Home** page.
- As the academic, I want to give the user an opportunity to view the publications and blogs I have featured in.
  - Both the **Publications** and **Blogs** pages are easily accesible through the navbar and contain relevant information about their associated posts.
- As the academic, I want to display all of my ongoing projects.
  - The **Projects** pages displays projects with their logos, giving visual feedback to the user, this page responds well on different screens and informs the user of the relevant details of the project.
- As the academic, I want to present contact details for both myself and other projects I'm involved in.
  - The **Contact panel** is accesible from every page and contains pertinent details to contact the academic through email, including a project she is heading.
- As the academic, I want to show my academic twitter feed.
  - The embedded twitter feed in the **Contact panel** allows a user of the site to see the three most recent tweets from the Academic. There is also a clear link leading the user to the academic's twitter feed.
- As a user, I want to get a general overview of the academic's achievements.
  - The **Home** page contains all the introductory details a user might want about the subject of the site.
- As a user, I want to access the articles and blog posts of this academic.
  - The easy to access **Publications** and **Blogs** pages which are in the nav allow a user to read through the academic's published works available online.
- As a user, I want to see what projects this academic is working on.
  - A user with a general interest in the academic's work can navigate to associated projects through the **Projects** page.
- As a fellow academic, I want to get in contact and enquire about collaboration.
  - Both the academic's email and the email of a project she is heading is easily accessible on all pages using the **Contact panel**.

## Bugs 

- As discussed previously the solution I used to apply an Alpha channel to a colour stored as a CSS variable threw an error in the validator. While the solution works visually and has the desired effect, a better solution I found uses PostCSS. As PostCSS is Javascript adjacent it's outside the scope of this project.
- While not necessarily a bug, I found during development that certain URLs were making my HTML files unwieldy. I opted to use bit.ly to shorten the URLs to make organising the source files easier.
- While validating the html files I discovered that I had left spaces in some og the file names which is undesirable, this was resolved by renaming the files.

[Return to README](README.md)