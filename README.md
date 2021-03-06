# allergens

## Setup

### Dependencies

- Run `npm install` in project directory. This will install server-related dependencies such as `express`.
- `cd client` and run `npm install`. This will install client dependencies (React).

### Database Prep

- Access the MySQL interface in your terminal
- Create a new database called facebook: `create database allergens`
- Add a `.env` file to the project folder of this repository containing the MySQL authentication information for MySQL user. For example:

```bash
  DB_HOST=localhost
  DB_USER=root
  DB_NAME=allergens
  DB_PASS=YOURPASSWORD
```

- Run `npm run migrate` in the project folder of this repository, in a new terminal window. This will create a tables called 'foodType' and 'restaurants' in your database.

### Development

- Run `npm start` in project directory to start the Express server on port 5000
- In another terminal, do `cd client` and run `npm start` to start the client in development mode with hot reloading in port 3000

_This is a student project that was created at [CodeOp](http://codeop.tech), a full stack development bootcamp in Barcelona._

- ## API endpoints

  ![API endpoints](/readmeImgs/APIroutes.png)

- ## Database layout

  ![Databases](/readmeImgs/database.png)

# Future Expansion Ideas

- add a log in feature so users can have a profile and save their favourite restaurants.

- add more search parameters: by delivery service, location, allergen.

- make it so each restaurant can have more than one type of food.

- add a carousel of images on each restaurant card.

- add a "see more restaurants" button to the all restaurants and search results pages, limiting the amount of cards that load at the beginning.
