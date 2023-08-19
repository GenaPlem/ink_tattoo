# INK TATTOO

INK TATTOO is a website designed to assist you in selecting and creating a unique tattoo design tailored to each client's preferences.
On our website, you can fill out a form to initiate a consultation with our manager.
You'll gain insights into our studio and have the opportunity to peruse a gallery showcasing our work process.
Furthermore, you can find answers to the most commonly asked questions in the FAQ section.

You can have a view by following this ---> [Link](https://genaplem.github.io/ink_tattoo/) <---

![Responsiveness of website](./README/images/website/responsiveness.png)

- - -

## Table of content
- [Description](#ink-tattoo)
- [Table of content](#table-of-content)
- [UX]()
- [Design](#design)
  - [Colors](#colors)
  - [Fonts](#fonts)
  - [Images](#images)
  - [Wireframes](#wireframes)
- [Testing](#testing)
  - [HTML validation](#html-validation)
  - [CSS validation](#css-validation)
  - [Lighthouse](#lighthouse)
  - [Known bugs](#known-bugs)
  - [Encountered Issues](#encountered-issues-during-development)
- [Credits]()

- - -
## Design

### Colors
- The color palette was carefully selected using the free palette creation service [Coolors.co](https://coolors.co/). The secondary color opacity was reduced to 30% for a dark red effect.

![Coolors.co palette generator](./README/images/design/colors_palette.png)

### Fonts
Two fonts are used on this website:
- **Druk Wide Cy Web** is used for the logo and headings in each section. It was downloaded from the free font repository [8font.com](https://8font.com/).
- **Inter** is used for the main body text. It was sourced from [Google fonts](https://fonts.google.com/).

### Images
- All images on this website were sourced from the free service [Freepik](https://www.freepik.com/).
They were then converted from PNG to WebP format using the free tool [Aconvert](https://www.aconvert.com/), and their sizes were optimized using [Tinypng](https://tinypng.com/)

### Wireframes
- I developed the website design using Figma, a collaborative design tool. The wireframes were created to visually plan the layout and user interface of the website before development began.

![Design wireframes top](./README/images/design/ink_tattoo_design_1.png)
![Design wireframes bottom](./README/images/design/ink_tattoo_design_2.png)
- - -
## Testing

### HTML validation
- No errors found with W3C validator.
  ![Html validation](./README/images/validations/html_validation_success.png)

### CSS validation
- No errors found with W3C.
  ![Css validation](./README/images/validations/css_validation_success.png)

### Lighthouse
- Achieved a perfect score of 100 in accessibility, performance, best practices, and SEO categories in both mobile and desktop versions.
  - Mobile Version:
    ![Lighthouse test mobile](./README/images/lighthouse/lighthouse_mobile.png)
  - Desktop Version:
    ![Lighthouse test desktop](./README/images/lighthouse/lighthouse_desktop.png)


### Manual testing
- The site has been thoroughly tested to ensure its compatibility and functionality across various scenarios:
  - The site has been tested on different operating systems, including Windows and macOS.
  - Testing has been conducted on different devices, including desktop computers, laptops, and mobile devices.
  - Compatibility has been verified across multiple browsers, such as Google Chrome, Safari, and Firefox.


- During manual testing, the following aspects were evaluated:
  - **Responsive Design:** The website's responsiveness was confirmed across various screen sizes and devices to ensure optimal user experience.
  - **Functionality:** All interactive elements, such as buttons, forms, and links, were tested to ensure they perform their intended actions.
  - **Cross-Browser Compatibility:** The website was tested on different browsers to identify and address any compatibility issues.
  - **Page Loading:** The loading times of different pages were measured to ensure quick and efficient loading.
  - **Navigation:** Navigational elements and menu options were tested to verify seamless navigation throughout the website.
  - **Form Submissions:** Form interactions were tested to ensure proper validation. As the form submissions are directed to a template provided by Code Institute, the testing focused on form interactions rather than actual submissions.


- As a result of comprehensive manual testing, the website has been validated for its consistent performance and user-friendly experience across diverse environments.

### Known Bugs
1. While extensive efforts have been made to ensure a smooth user experience, there is a known issue with the form's phone number validation due to the limitations of this project being solely developed using HTML and CSS. Since JavaScript is not employed in this project, advanced form validations, such as phone number formatting, cannot be achieved.

   - **Issue:** Phone number validation is not enforced due to the absence of JavaScript.
   - **Impact:** Users may input phone numbers in various formats that do not conform to the expected pattern.


2. Despite careful development, a known issue affects the menu's behavior. Currently, the menu doesn't close when users click outside the menu area. It can only be closed using the close icon, which can lead to suboptimal user experience.
    - **Issue:** The menu does not close when clicking outside the menu area.
    - **Impact:** Users might find it inconvenient to only close the menu using the dedicated close icon, which could negatively affect user experience.

### Encountered Issues During Development

While developing the project, several issues were encountered and resolved.
1. One notable challenge was related to the initial navigation menu, which relied on hover interactions within an unordered list. However, this approach proved ineffective on the mobile version when were deployed on github pages and tested on mobile phone.
   - **Issue:** The initial menu design using hover interactions on an unordered list didn't work as expected on mobile devices.
   - **Resolution:** The issue was addressed by implementing a`input[type=checkbox]`to control the menu. This ensured consistent behavior across both desktop and mobile devices, enhancing user accessibility and experience.


2. Second issue arose when implementing dynamic width `100dvw` for a map container. In specific browser scenarios where the scroll bar consumes a portion of the screen width, the scroll bar width was not properly accounted for. This resulted in a horizontal scroll appearing in the screen width range from ```768px``` to ```1024px```.
   - **Issue:** The dynamic width (dvw) applied to the map container didn't account for the width of the scroll bar in browsers where it occupied screen space, leading to an unintended horizontal scroll between `768px` and `1024px`.
   ![Horizontal scroll issue](./README/images/issues/issue_hr_scroll.jpg)
   - **Resolution:** To mitigate this issue, the decision was made to restrict horizontal scrolling by applying `overflow-x: hidden;` to the entire content. While this resolved the horizontal scrolling problem, a small portion of the map might be hidden beneath the scroll bar. This trade-off was made in favor of a better user experience.
   ![Horizontal scroll resolution](./README/images/issues/fixed_hr_scroll.jpg)


3. Third issue that emerged during testing with the W3C CSS Validator was related to an animation effect applied on hover to the links within the menu on the desktop version. The validator reported an error stating `Property scale doesn't exist.`
   - **Issue:** The hover animation effect applied to menu links on the desktop version raised an error in the W3C CSS Validator, reporting that the property "scale" doesn't exist.
   ![W3C CSS validation error](./README/images/validations/css_validation_error.png)
   - **Resolution:** To address this issue, the approach was adjusted by using the transform property with the scale function. The animation effect was achieved by applying `transform: scale();` instead of `scale()`.
- - -
