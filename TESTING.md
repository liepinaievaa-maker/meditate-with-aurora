+ ## Testing

+ Extensive testing was carried out throughout the development process to ensure that the Aurora Meditation website functions correctly, is visually consistent, and provides a smooth user experience across different devices and browsers.

+ The site has been tested manually on various screen sizes and browsers to confirm that all features work as intended and that users can easily achieve their goals — whether it’s reading about Aurora, meeting the team, or booking a session.

 ### General Functionality Testing

  + All navigation links across the site work correctly and lead to the intended pages or sections.
  + The fixed navigation bar remains visible and functional during scrolling.
  + The hero section image loads properly on all devices, with responsive text and working call-to-action button.
  + The “About” section displays correctly with images aligned as intended and text remaining readable at all breakpoints.
  + The “Team” page cards are responsive and visually balanced.
  + The “Booking” page form accepts input, validates required fields, and successfully redirects to the success confirmation page.
  + The “Success” page correctly confirms submission and links back to the homepage.
  + Footer social media icons open in a new tab and direct users to the correct platforms.
  + All components were also tested for proper alignment, spacing, and font rendering on both desktop and mobile devices.
---

 ### Browser and Device Compatibility
+ The project was tested on the following browsers and operating systems:
  + Google Chrome (Desktop & Mobile)
  + Mozilla Firefox
  + Microsoft Edge
  + Safari (iOS)

+ All pages displayed as expected on:
  + Desktop (Full HD & 4K)
  + Tablet (768px width)
  + Mobile Devices (480px and smaller)

+ The website’s responsiveness was verified using Chrome DevTools and actual physical devices to ensure consistent layout behavior across breakpoints.
---
 ### Performance and Accessibility

+ Performance, accessibility, and best practices were tested using Google Lighthouse.
The site scored highly in all categories, confirming that the structure, contrast ratios, and meta tags are well-optimized.

+ Accessibility was also reviewed manually:
  + All images include descriptive alt attributes.
  + Proper heading hierarchy (h1, h2, h3, etc.) is maintained across pages.
  + Links and buttons are clearly distinguishable and include hover feedback.

![Lighthouse on device main page](documentation/lighthouse-device-main-page.PNG)
![Lighthouse on device team page](documentation/lighthouse-device-team-page.PNG)
![Lighthouse on device booking page](documentation/lighthouse-mobile-booking.PNG)
![Lighthouse on device success page](documentation/lighthouse-device-success-page.PNG)
![Lighthouse on mobile main page](documentation/lighthouse-mobile-home-page.PNG)
![Lighthouse on mobile booking page](documentation/lighthouse-mobile-booking.PNG)
---
 ### Validator Testing

+ HTML 
  + All pages were tested using the [W3C Markup Validation Service](https://validator.w3.org/nu/?doc=https%3A%2F%2Fliepinaievaa-maker.github.io%2Fmeditate-with-aurora%2Findex.html)
  + No errors or critical warnings were returned.
![HTML validator results](documentation/html-validator.PNG)

+ CSS
  + The CSS file was validated using the [W3C Jigsaw CSS Validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fliepinaievaa-maker.github.io%2Fmeditate-with-aurora%2Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=el)
  + The stylesheet has no errors, only minor warnings about CSS variables and vendor prefixes (which are normal and acceptable in modern web design) and they mostly are because of used Bootstrap.
![CSS validator results](documentation/css-walidator.PNG)
---
### Manual Testing
| Hero Section |||||
| Hero image | Load homepage | Image covers full width and adjusts to screen size | Yes | Yes | Minor adjustments made to fix white space bug |
| Hero text | View on different screen sizes | Text remains centered and readable | Yes | Yes | Adjusted padding and font size for mobile |
| “Booking” button | Click the button | User is redirected to Booking page | Yes | Yes | Works as intended |

| About Section |||||
| About images | View on desktop and mobile | Images resize and align properly | Yes | Yes | Optimized using Squoosh for faster loading |
| About text | Read text content | Text is readable and balanced on all screens | Yes | Yes | Responsive layout confirmed |

| Team Page |||||
| Team cards | View all team members | Cards are displayed evenly in grid format | Yes | Yes | - |
| Card images | Hover over image | Image remains centered; no distortion | Yes | Yes | - |
| Booking button on each card | Click “Booking” button | User is redirected to Booking page | Yes | Yes | - |

| Booking Page |||||
| Name input | Enter text | Text appears correctly | Yes | Yes | Required field works |
| Phone input | Enter numbers | Input accepted | Yes | Yes | - |
| Email input | Enter valid/invalid email | Valid email accepted; invalid rejected | Yes | Yes | Browser validation works |
| Teacher dropdown | Select guide from list | Option selected correctly | Yes | Yes | - |
| Message area | Type message | Text appears and scrolls correctly | Yes | Yes | - |
| Submit button | Click “Submit” | User redirected to Success page | Yes | Yes | - |

| Success Page |||||
| Confirmation message | Load success page | “Thank you” message displayed clearly | Yes | Yes | - |
| Return button | Click “Return to Home Page” | Redirects back to homepage | Yes | Yes | Works smoothly |

| Footer |||||
| Facebook icon | Click icon | Opens Facebook in new tab | Yes | Yes | Uses target="_blank" correctly |
| Instagram icon | Click icon | Opens Instagram in new tab | Yes | Yes | - |
| YouTube icon | Click icon | Opens YouTube in new tab | Yes | Yes | - |
| Contact info | View text | Address, email, and phone readable and clickable | Yes | Yes | Consistent across all pages |
---

 ### Bugs

+ Although the website works well overall, a few small issues were discovered during development and testing:

  + Hero Image Width Issue:

    + The main hero image initially appeared too wide on larger screens, slightly extending beyond the viewport and causing unwanted horizontal scrolling.
    + My goal was to have the image fill the entire width of the screen without leaving any white borders — but this occasionally conflicted with Lighthouse’s layout and responsiveness requirements.
    + After several adjustments to object-fit and object-position, the issue was minimized, and the image now displays correctly across all major devices.  
    + However, a very small discrepancy remains at some unusual screen sizes, which I plan to perfect in future updates.

  + Image Optimization for Lighthouse Performance:

    + Early Lighthouse tests showed a slightly reduced performance score due to large image file sizes.
    + To fix this, I used the external website [Squoosh](https://squoosh.app/) to compress and resize all images without losing quality.
    + After optimization, the site loads much faster, and the Lighthouse performance score improved significantly.

+ A few areas have been noted for improvement in future development:

  + Bootstrap Navbar Responsiveness:
    + During testing, minor layout issues appeared on certain screen widths (particularly between 768px–992px). These are caused by Bootstrap’s predefined flex behaviors. The plan is to rebuild the navigation bar from scratch in the future for more predictable styling.

  + Bootstrap Booking Form Layout:
    + Some alignment inconsistencies occur when resizing the window rapidly. This issue also stems from Bootstrap’s grid system. A fully custom-built booking form will replace this version to ensure smoother responsiveness.

+ No functional bugs remain unresolved, and all interactive elements currently work as intended.
