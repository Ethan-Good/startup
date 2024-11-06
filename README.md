# startup
startup application for CS 260

[Notes](notes.md)

## Specification Deliverable

### Elevator pitch

Tekken is one of the most difficult fighting games to learn. Each of the 30+ characters have more than 100 different moves, some even having 200. For a new player this amount of moves can be incredibly overwelming. This is where the Tekken Database comes in. On this website there will be images of the most important moves from each character and how to beat them. Users can login, select the character they are having trouble beating and learn their most common moves. Users can also add matchup specific advice for the character they play. Its the one stop shop for learning how to beat any character in Tekken 8.

### Design

![Design](mock.jpg)

### Technologies

I am going to use the required technologies in the following ways.

- **HTML** - There will be several HTML pages, one for each character and a home page. Each page will have a few gifs of the characters most important moves.
- **CSS** - I will use this application to style the website and make it look good.
- **React** - Provides login, choice display, applying user matchup advice, and use of React for routing and components.
- **Service** - Backend service with endpoints for:
  - login
  - submitting matchup advice
- **DB/Login** - Store users and matchup advice in database. Register and login users. Can't add matchup advice unless authenticated.
- **WebSocket** - As each user adds matchup advice, it will broadcast it all users.

## HTML deliverable

For this deliverable I coded the structure of my website using HTML.

- **HTML pages** - I have 5 html pages. A home page where a user can login, an about page where they can learn about the website and 3 character pages.
- **Links** - Each page has a header that has links to all the other pages.
- **Text** - I have lots of text to teach people how the website works and information about character moves.
- **Images** - I have several images including an icon on the tab at the top.
- **DB/Login** - I have an input box and submit button for people to login.

## CSS deliverable

For this deliverable I styled my website into its final appearance.

- **Header, footer, and main content body** - I made the header, footer and body a different color on the home page
- **Navigation elements** - I made the navbar stick to the top to have more room on screen
- **Responsive to window resizing** - My app looks great on all window sizes and devices
- **Application elements** - Used good contrast and whitespace using margins
- **Application text content** - Consistent fonts
- **Application images** - I styled my pictures to have rounded edges and be spaced apart with padding
