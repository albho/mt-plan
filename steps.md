# Start

1. See 'Getting Started' section in README.md file of Resource-Wall project directory

# Backend

## Database

1. /db/schema: create tables based on ERD
2. /db/seeds: seed data
3. run `npm run db:reset`

## Routes

1. GET /resources

   - render all posts by all users
   - display all info + number of likes, number of comments
   - search feature

2. GET /resources/liked

   - render all posts by liked by current user

3. GET /resources/owned

   - render all posts by owned by current user

4. GET /resources/new

   - form to create new resource

5. POST /resources

   - create new resource, redirect to /resources/:id

6. GET /resources/:id/update

   - form to update resource

7. POST /resources/:id/update

   - update resource, redirect to /resources/:id

8. POST /resources/:id/delete

   - delete resource, redirect to /resources

**User**

9. GET /login

   - email, password

10. POST /login

    - email, password

11. POST /logout

    - clear cookie

12. GET /register

    - email, password

13. POST /register

    - email, password

14. GET /user

    - show user details

15. POST /user/:id

    - form to update username, delete account

# Frontend

## Views

1. **navbar.ejs** (partial)

2. **index.ejs**

   - default home page
     - GET /resources
     - GET /resources (with search results)
   - current user's liked resources
     - GET /resources/liked
   - current user's owned resources
     - GET /resources/owned

3. **view_resource.ejs**

   - specific post
     - GET /resources/:id

4. **create_resource.ejs**

   - form
     - GET /resources/new
     - POST /resources
     - POST /resources/:id/update
     - POST /resources/:id/delete

5. **auth.ejs**

   - form
     - GET /login
     - POST /login
     - GET /register
     - POST /register

6. **user.ejs**

   - user details
     - GET /user
   - form
     - POST /user/:id

## jQuery

- Navbar
  - Home (GET /resources)
  - Login (GET /login)
  - Logout (GET /logout)
  - Username
  - My Submitted Resources (GET /resources/owned)
  - My Liked Resources (GET /resources/liked)
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
- Resource thumbnail? Add to ERD
- Auth requirements?
- Ability to edit resources? /resources/:id/edit
- not sure if routes /resources/liked and /resources/owned follow naming convention?
- /resources/new and /resources/:id/edit can use the same view template
