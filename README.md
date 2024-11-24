# Yubaba

[View deployed site] (https://krisjowen.github.io/yubaba/index.html)

This site has been built as the first of four projects as part of my Code Insitute web development diploma. It is a website for a band that provides images and videos to showcase their work as well as a booking form for any interested clients to get in touch with them.


# UX

## Strategy

The user stories were defined as follows:

- As a site visitor, I want to be able to see details about the band and to contact them with details of any potential bookings.
- As the band, I want to show images of how we look and present a profile

The acceptance criteria were outlined as below:

- High quality image of band available
- Booking form in place
- Profile of band and its members

## Scope

Decision to use a four page website. Future developments could include gig list, set lists and a more elaborate booking form

## Structure

Include sitemap

## Skeleton

Include wireframes

## Surface

Font and colour choices, hero image, videos, 

# Features

## Existing Features

## Future improvements

# Technologies Used

* [HTML](https://html.spec.whatwg.org/)
* [CSS](https://www.w3.org/TR/CSS/#css)
* [Bootstrap](https://getbootstrap.com/) - Bootstrap was utilised for various aspects including, but not limited to, the nav bar, carousel, form and member profile cards
* [Google Fonts](https://fonts.google.com/specimen/Abel) - the Abel and Macondo Google fonts have been used throughout this project
* [Font Awesome](https://fontawesome.com/) - the social icons in each page's footer are from Font Awesome
* [Balsamiq](https://balsamiq.com/) - the wireframes for this project were constructed using Balsamiq
* [Git](https://git-scm.com/) - Git was utilised for version control via Gitpod
* [Github](https://www/github.com) - utilised to store the various versions of the project uploaded via Gitpot  
* [Image Compressor](https://imagecompressor.com/) - used to compress images and reduce their file size


# Testing

## Links

All links have been tested to ensure they route through to the correct location.

### Navbar

The navbar has been tested on each of the four pages to ensure it links correctly throughout. The logo in the navbar also links to index.html throughout

### Footer

Across all four pages the four social links within the footer link through to the correct social media link

### Buttons

The various buttons across the site link correctly. There are three variations

* Book Us - this links through to contact.html where it appears
* Submit - this appears on contact.html and links to success.html
* Return to the home page - this is available on success.html and correctly links through to index.html

## Responsiveness

Responsiveness has been tested with Google Chrome dev tools and emulating various device settings.

## Lighthouse

Page | Performance | Accessibility | Best Practices
--- | --- | --- | ---
index.html | 82 | 100 | 78
about.html | 78 | 100 | 100
contact.html | 91 | 96 | 78
succcess.html | 98 | 95 | 78

### index.html

The 82 for performance is attributed to the hero image having a long render delay. Despite several attempts to reduce the image size I was unable to bring this down to an acceptable level. The 78 best practices score was due to third party cookies that were introduced with the Youtube embed code.

### about.html

The 78 for performance was similar to the index.html page in that I was unable to bring the render delay for some of the page images down to a respetable level.

### contact.html

Similarly to the index.html page the best practices score is 78 due to the cookies that are brought in the with the embedded Youtube code

### success.html

The 78 score is again due to the cookies from the Youtube embedded code


# Deployment

Github Pages

# Credits

On each html page there is a section of code with the below comment:

Class set on body to work with mt-auto in footer to ensure it always stays at the bottom of the page

This code was taken directly from the Code Institute's Boardwalk Games page found [here](https://github.com/Code-Institute-Solutions/boardwalk-games-v1-sourcecode)