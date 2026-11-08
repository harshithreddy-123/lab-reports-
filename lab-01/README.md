# Lab 1: Node.js and Express server

**Name:** G Harshith Reddy 
**Registration number:** 252U1R6078
**Section:** AIML-2B / 207 

## Live link
https://dp-lab-01.onrender.com

## Objective
Create a basic server using Node.js built-in `http` module, then create an Express server with three GET routes and a 404 response for unknown paths.

## How to install and run
1. Install Node.js and npm.
2. Open a terminal in this `lab-01` folder.
3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the Express server:

   ```bash
   npm start
   ```

5. Open `http://localhost:3000` in your browser.

To run the plain Node.js HTTP server instead, stop the Express server with `Ctrl + C`, then run:

```bash
npm run start:plain
```

No environment variables are required for this lab.

## Endpoints

| Method | Path | Description | Expected status |
|---|---|---|---|
| GET | `/` | Returns a welcome message | 200 |
| GET | `/about` | Returns name and section as JSON | 200 |
| GET | `/time` | Returns the current date and time | 200 |
| GET | Any unknown path | Returns a not-found message | 404 |

## Screenshots

### Home route (GET /) - status 200
![Home route returning welcome message with status 200](screenshots/home.png)

### About route (GET /about) - status 200
![About route returning JSON with name and section](screenshots/about.png)

### Time route (GET /time) - status 200
![Time route returning current date and time](screenshots/time.png)

### Unknown route - status 404
![Unknown path returning 404 Page not found](screenshots/not-found.png)

### Plain Node.js http server
![Plain http server replying Hello](screenshots/plain-hello.png)

### Status codes returned
| Route | Status |
|---|---|
| `/` | 200 |
| `/about` | 200 |
| `/time` | 200 |
| `/unknown` | 404 |


