# Yubaba

[View deployed site](https://krisjowen.github.io/yubaba/index.html)

This site has been built as the first of four projects as part of my Code Insitute web development diploma. It is a website for a band that provides images and videos to showcase their work as well as a booking form for any interested clients to get in touch with them.

The band currently have a wordpress website built by one of the members. There is a desire to move away from Wordpress to allow for greater customisation and potentially more features in the future.

# UX

## Strategy

The user stories were defined as follows:

- As a site visitor, I want to be able to see details about the band and to contact them with details of any potential bookings.
- As the band, I want to show images of how we look and present a profile

The acceptance criteria were outlined as below:

- High quality image of band available
- Booking form in place
- Profile of band and its members
- Site is responsive

## Scope

In order to achieve a mvp it has been decided that the site should allow any potential customers to get both video and visual indications of what the band's style is. Additionally, any site users should be able to utilise a form to get in touch with the band with any potential booking inquiries. 

## Structure

A basic structure has been defined which can be seen [here](https://github.com/krisjowen/yubaba/blob/main/assets/wireframes/Sitemap.png).

Inline with the user stories and acceptance criteria, the structure at present has been decided as the below:

- Home (index.html) - a basic landing page with an image of the band and a video
- About (about.html) - a section with details of the band and individual member profiles
- Contact (contact.html) - a page containing a form for any interested parties to get in touch
- Message confirmation (success.html) - a page informing a user their message has been sent

Additionally, each page should have an easy to use navigation bar to move around the site and a footer containing links to the band's various social media pages.

## Skeleton

Wireframes to produce a draft of what each page should look like were created using Balsamiq:

- [index.html](https://github.com/krisjowen/yubaba/blob/main/assets/wireframes/Home.png)
- [about.html](https://github.com/krisjowen/yubaba/blob/main/assets/wireframes/About.png)
- [contact.html](https://github.com/krisjowen/yubaba/blob/main/assets/wireframes/Contact.png)
- [success.html](https://github.com/krisjowen/yubaba/blob/main/assets/wireframes/Success.png)

The desire is to keep the content on the pages relatively clean and let the visual aspects do the talking.

## Surface

### Font

The band had an existing Wordpress website that utilised the 'Abel' Google font. This looked to be working well and so this has also been utilised here.

### Colours

The band's current website is somewhat dark and moody. In order to attract more bookings a decision has been made to introduce a more inviting and colourful palette. Pastel blues and yellow were used and these complement the band's existing images well. 

### Media

The band already had possession of a number of high quality images and these were seen as an effective way to showcase their look and style. Additionally, some of their videos are available on Youtube so this was seen as a simple way to display some of their content. They also have music available on Spotify but the added benefit of having visual content via Youtube was seen as a preference. 

# Features

## Existing Features

### Global Features

- A navigation bar is fixed to the top of the page to help users find their way around the site
- The band's logo is visible at the top left of the page at all times and links to index.html
- To keep the site responsive and help with mobile users the nav bar links collapse into a hamburger menu at smaller screen sizes
- The footer contains links to the band's social media pages. These utilise images from Font Awesome and open in a new tab

### index.html

- The hero image has been set at 100% of the viewport height to give maximum visual impact when landing on what is the home page
- The band's logo is laid over the hero image to increase the visibility of whose site it is to any users
- The band logo disappears at smaller screen sizes as it is superfluous due to the logo in the nav bar when viewing at a smaller size
- A book us button is immediately visible on any screen size as that is the main outcome the band want from site visitors
- A Youtube video is embedded beneath the hero image

### about.html

- Bootstrap has utilised to present two rows of responsive content. The first row contains a band profile and a carousel of images whilst the second contains individual member profiles
- A carousel displays four images of the band in action
- Six Bootstrap cards are used to display individual images of each band member and a short profile

### contact.html

- Bootstrap has again been used to present a responsive page. The rows are for the text section and video and a second row for the booking form
- A Youtube video is embedded to showcase the bands content
- A simple contact form is in place to capture any interested user's name, email address, type of event, date and a text area for any additional information. The name, email and date fields have been marked with asterisk to denote them being mandatory

### success.html

- A short text message thanks the user for their form submission
- A Youtube video is in place to further showcase the band's content
- A button links back to the homepage

## Future improvements

### Additional Content

#### Gig List

To further attract user engagement a list of the band's upcoming performances would be a good addition. This could form part of the home page or be an additional page. It would require ongoing maintenance, however, and so calendar integrations may need to be considered so that updating the list could be handled in a low-tech manner.

#### Audio Content

There is good content already in place to display the band's output. However, it would be useful to look at ways of including audio clips or songs. Spotify offers an embedded code and the band's music is on there but the integration potentially lacks customisation options.

### Bugs

#### Navbar Link Styling

To aid user navigation hover and active stylings have been added to the nav bar links. Whilst these work well and clearly show which page a user is currently on and which option they are hovering over, the implementation could be improved. The CSS for this is below:

.active {
    background-color: rgba(0,0,0,0.5) !important;
    color: var(--primary-color) !important;
  }

I would prefer to find a solution that does not target .active globally but is restricted to the nav bar links. I would also like to find a solution that does not require use of the !important due it not generally being considered best practice to utilise it.

# Technologies Used

- [HTML](https://html.spec.whatwg.org/)
- [CSS](https://www.w3.org/TR/CSS/#css)
- [Bootstrap](https://getbootstrap.com/) - Bootstrap was utilised for various aspects including, but not limited to, the nav bar, carousel, form and member profile cards
- [Google Fonts](https://fonts.google.com/specimen/Abel) - the Abel and Macondo Google fonts have been used throughout this project
- [Font Awesome](https://fontawesome.com/) - the social icons in each page's footer are from Font Awesome
- [Balsamiq](https://balsamiq.com/) - the wireframes for this project were constructed using Balsamiq
- [Git](https://git-scm.com/) - Git was utilised for version control via Gitpod
- [Github](https://www/github.com) - utilised to store the various versions of the project uploaded via Gitpot  
- [Tiny PNG](https://tinypng.com/) - used to compress images and reduce their file size
- [Auto Prefixer](https://autoprefixer.github.io/) - this site helps with browser compatibility by adding different browser prefixed to the style.css file where required


# Testing

## Code Validation

All pages were put through the below validation tools and returned no errors:

- [HTML Validator](https://validator.w3.org/)
- [CSS Validator](https://validator.w3.org/)

## Links

All links have been tested to ensure they route through to the correct location.

### Navbar

The navbar has been tested on each of the four pages to ensure it links correctly throughout. The logo in the navbar also links to index.html throughout

### Footer

Across all four pages the four social links within the footer link through to the correct social media link

### Buttons

The various buttons across the site link correctly. There are three variations

- Book Us - this links through to contact.html where it appears
- Submit - this appears on contact.html and links to success.html
- Return to the home page - this is available on success.html and correctly links through to index.html

## Responsiveness

Responsiveness has been tested with Google Chrome dev tools and emulating various device settings. This has ensured that all content remains accessible and easily viewable regardless of screen size.

## Lighthouse

Page | Performance | Accessibility | Best Practices
--- | --- | --- | ---
index.html | 88 | 100 | 78
about.html | 88 | 100 | 100
contact.html | 99 | 100 | 78
succcess.html | 98 | 100 | 78

### index.html

The 88 for performance is attributed to the hero image having a long render delay. The 78 best practices score was due to third party cookies that were introduced with the Youtube embed code.

### about.html

The 88 for performance was similar to the index.html page in that I was unable to bring the render delay for some of the page images down to a better level. The page contains 10 images that have all been compressed using Tiny PNG.

### contact.html

Similarly to the index.html page the best practices score is 78 due to the cookies that are brought in the with the embedded Youtube code

### success.html

The 78 score is again due to the cookies from the Youtube embedded code

## Browser Compatibility

All pages and functionality have been tested in Google Chrome, Firefox and Safari and show expected and consitent results in each browser

# Deployment

## Deploying to Github Page

The project was monitored by utilising the Github pages feature. This was created using the below steps:

1. From the [main project page](https://github.com/krisjowen/yubaba), click on the settings tab
2. Choose 'Pages' from the menu on the left
3. Under Build and Deployment and then Branch, main and then root were selected and the options saved
4. Once created, from the main project page again there is a 'Deployments' option on the right hand menu. This shows the URL for the Github Page

## Cloning Project

Details of this can be found on Github's own [documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

1. Within Github, navigate to the [main page](https://github.com/krisjowen/yubaba) of the repository
2. Above the list of files, click on the green 'Code' button
3. For HTTPS integrations, copy the web url given under the 'Local' tab
4. Within your terminal, navigate to the desired file path. 
5. Type git clone then paste the code that has been copied (https://github.com/krisjowen/yubaba.git) and hit enter.

# Credits

On each html page there is a section of code with the below comment:

Class set on body to work with mt-auto in footer to ensure it always stays at the bottom of the page

This code was taken directly from the Code Institute's Boardwalk Games page found [here](https://github.com/Code-Institute-Solutions/boardwalk-games-v1-sourcecode)