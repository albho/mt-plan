# Start

1. See 'Getting Started' section in README.md file of Resource-Wall project directory

# Backend

## Database

1. /db/schema: create tables based on ERD
2. /db/seeds: seed data
3. run `npm run db:reset`

## Routes

1. GET /

   - render all posts by all users
   - display all info + number of likes, number of comments
   - search feature
   - jQuery to filter likes and owned
   - jQuery to toggle comments
   - form to create new resource

2. POST /resources

   - create new resource, redirect to /resources/:id

<!-- 6. GET /resources/:id/update

   - form to update resource -->

<!-- 7. POST /resources/:id/update

   - update resource, redirect to /resources/:id -->

<!-- 8. POST /resources/:id/delete

   - delete resource, redirect to /resources -->

<!-- 1. POST /login

   - email, password -->

1. POST /login/:id

- email, password

2. POST /logout

   - clear cookie

<!-- 4. GET /register

   - email, password

5. POST /register

   - email, password

6. GET /user

   - show user details

7. POST /user/:id

   - form to update username, delete account  -->

# Frontend

## Views

1. **index.html**

   - navbar
     - POST /login
     - POST /logout
   - default home page
     - GET /resources

   - **drop-down form**
     - POST /resources
     <!-- - POST /resources/:id/update
     - POST /resources/:id/delete -->

<!-- 3. **view_resource.ejs**

   - specific post
     - GET /resources/:id -->

<!-- 4. **auth.ejs**

   - form
     - GET /login
     - POST /login
     - POST /logout
     - GET /register
     - POST /register

5. **user.ejs**

   - user details
     - GET /user
   - form
     - POST /user/:id -->

## jQuery

- Navbar
  - Home (GET /resources)
  - Login (POST /login)
  - Logout (POST /logout)
  - Username
- Etc. for each page & component

## CSS

- Sass + (Bootstrap or Tailwind)
- File organization: follow
  https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Organizing
- Responsive

## Stretch (Optional)

- Hosting, such as heroku, netlify, github pages, AWS, or Azure

### Questions & Considerations

- How best to group routes into different files?
- Delete branch after it has been merged?
