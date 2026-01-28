# Library Ace

[Library Ace](https://startup.libraryace.click)

This application allows a user to select and "ace" one book. After a user selects their favorite title, the favorite count is added to for that book. Users are able to see the most loved books, allowing them to find their next read. Users can browse through the selection of books, gaining valuable information such as title, author, and summary.

### Elevator pitch

Done with reading books that are just okay? Done with searching through ratings and videos to find a book worth your time? Through Library Ace, you can find the best of the best! Each user gets one book to favorite, and that's it! Choose your favorite book that you think everyone needs to read and you will be helping others find only the best books. See what books are the most beloved in the community, and find something that is worth your time to read.

### Design

![Design image](libraryaceMyAcePage.png)

### Key features

- Secure login over HTTPS
- Ability to favorite a most-loved book
- Stores and totals favorites
- Displays basic title information

### Technologies

Library Ace uses these technologies in the following ways.

- **HTML** - Uses correct HTML structure for application. Three HTML pages. One for login, one for books, one for rankings. Hyperlinks to choice artifact.
- **CSS** - Application styling that looks appropriate on different screen sizes, uses good whitespace, color choice and contrast.
- **React** - Provides login, applying favorite, display other users favorites, and use of React for routing and components.
- **Service** - Backend service with endpoints for:
    - login
    - submitting favorite
    - retrieving favorites status
- **API** - Uses Google Books API to get book information such as title, author, cover, and summary.
- **DB/Login** - Stores users and favorites in database. Register and login users. Credentials securely stored in database. Can't vote unless authenticated.
- **WebSocket** - Most recent favorited books are displayed in real-time.

## 🚀 AWS

- [x] **Server deployed and accessible with custom domain name** - [Library Ace](https://startup.libraryace.click).

## 🚀 HTML

- [x] **HTML pages** - Created a home page, a book page, and a ranking page.
- [x] **Proper HTML element usage** - Used headers, menu, table, and more elements throughout the HTML.
- [x] **Links** - Links to each available page, project GitHub, and an image link all properly utilized.
- [x] **Text** - Text is all filled in, with some generic text being used to represent a summary or title.
- [x] **3rd party API placeholder** - Book information was left intentionally blank, as API will fill this information in.
- [x] **Images** - Image of a book properly displayed and given alt text on My Book page.
- [x] **Login placeholder** - Both username and password taken. Once logged in, taken to My Book HTML page.
- [x] **DB data placeholder** - Top favorited books are shown in a table in the rankings page.
- [x] **WebSocket placeholder** - Recently favorited books and who favorited them are shown on the rankings page.

## 🚀 CSS

- [x] **Header, footer, and main content body** - All HTML content is formatted and present.
- [x] **Navigation elements** - Navigation bar sends user to all pages, and shows active page.
- [x] **Responsive to window resizing** - Window can be resized to show all content, no content is hidden by navigation bar when resizing.
- [x] **Application elements** - Created consistent coloring and branding, charts and buttons.
- [x] **Application text content** - Text is thoughtfully designed and formatted with CSS and colored.
- [x] **Application images** - Created a custom button that matches Bootstrap buttons but with Library Ace brand colors.

## 🚀 React part 1: Routing

- [x] **Bundled using Vite** - Correctly bundled program using Vite, matching expected format.
- [x] **Components** - All HTML components have been transfered over.
- [x] **Router** - Routinged between login and voting components correctly.

## 🚀 React part 2: Reactivity

- [x] **All functionality implemented or mocked out** - Book aces are tallied for each book, repeteatable for uders. Login is functional. Websocet capabilities are mocked.
- [x] **Hooks** - UseState manages component-level state and useEffect runs when things change.

## 🚀 Service

- [x] **Node.js/Express HTTP service** - Node.js and Express HTTP implemented.
- [x] **Static middleware for frontend** - Middleware in auth and use was correctly completed.
- [x] **Calls to third party endpoints** - Sent calls to Google Books API for book information.
- [x] **Backend service endpoints** - Endpoints for all actions such as login/create/logout, aces, and more.
- [x] **Frontend calls service endpoints** - Frontend calls for login page and ace information.

## 🚀 DB/Login

- [x] **User registration** - User is saved in MongoDB when creating an account.
- [x] **User login and logout** - User login information is pulled from MongoDB with a hashed password. When logged out, user must log back in to continue session.
- [x] **Stores data in MongoDB** - User ace information is stored alongside their credentials. When a book is aced, the book is added to MongoDB with it's own information.
- [x] **Stores credentials in MongoDB** - User username, password, and token are stored in MongoDB.
- [x] **Restricts functionality based on authentication** - Login page is only page available when unauthenticated. When authenticated, user is able to access all pages.

## 🚀 WebSocket

- [x] **Backend listens for WebSocket connection** - Backend listens for a recent ace.
- [x] **Frontend makes WebSocket connection** - Frontend makes a WebSocket connection to the backend to grab data.
- [x] **Data sent over WebSocket connection** - Username and book ace title are sent over WebSocket.
- [x] **WebSocket data displayed** - UI displays the username and their book ace in a table. It automatically only shows five at a time, updating as they come through.
- [x] **Application is fully functional** - Library Ace is fully functional! Secure authentication is implemented. Users are able to search and select one book ace. Users can see the most highly and more recent aces.

### Notes

The following link takes you to notes that specify technologies or processess I found interesting while developing in each technology stack section.

[My Notes](notes.md)
