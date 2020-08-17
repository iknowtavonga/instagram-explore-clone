# Instagram Explore Page

## Project motivation

After learning css grid through tutorials i decided to implement the concept i had learnt in a project. I used css grid in my previous project (2020 August Portfolio) but to solidify this concept i had to create a project which is centered on grids. This lead me to choosing Instagram. 

The following questions determined how i was going to implement the project while simultaneously grasping the concept of grids. 

* which section am i going to clone
* am i going to clone the web version alone or the app version alone or both
* am i going to implement the grid across the full page or the main section alone
* am i going to simulate a logged in or logged out account

## Contributors
* Tavonga I Karimanzira

## Web version

The web version of this explore page does not contain any videos and this made the grid 

### Header

The header was flexed to allow for an equal amount of space between the following items:
* Logo
* Search bar
* Login and sign up buttons

### Main

The main section contains a combination of 3x2 grids along with a title separating recent images and top posts.

## App version

The app version was a little more complicated than the web version as it had more grid elements included along with a sticky header and fixed footer. If more time arises i might optimise the app version for tablet devices because the elements look stretched on those devices.

### Header
#### Header Top
* Search bar
* Scan button

#### Header Bottom

The header bottom sticks to the top of the screen when the user scrolls down
* hashtag buttons

### Main

* Reels video
* Pictures only grid
* Pictures and video grid
* Pictures only grid

The grid system is separated into different groups as shown above. This is not a nested grid system but individual grid systems that have been combined to make one whole grid. 

### Footer
The footer is fixed to the bottom of the page and flexed to keep the icon distant equal. The following icons are used in the footer:
* Home
* Search
* Upload
* Likes
* User

## Hardest sections

Grid templates have been tricky for me and this project pushed me to the deep end and forced me to learn and understand the concept better. I am still a few projects away from being comfortable with the concept but the learning process has been an interesting one. The following code shows how i executed my video and pictures grid...

```css
    .pv-container{
        margin: 3px;
        display: grid;
        grid-gap: 3px;
        grid-template-areas: 
        'top-pv-image pv-video pv-video'
        'bottom-pv-image pv-video pv-video';
    }

    .pv-video{
        grid-area: pv-video;
    }

    .video{
        height: 30vh;
        width: 64vw;
    }

    .top-pv-image{
        grid-area: top-pv-image;
        width: 32vw;
    }

    .bottom-pv-image{
        grid-area: bottom-pv-image;
        width: 32vw;
    }
```