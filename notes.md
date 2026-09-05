YouTube tutorial: https://www.youtube.com/watch?v=F9gB5b4jgOI&list=PLFacaW1gAylpxwtV7TPf_NRWR5cM86eFS

MERN stack notes: https://app.eraser.io/workspace/GlhY2F7ltehsjZ2z9phZ

MERN stack
- MongoDB: database
    - place where you store the data
- Express: web framework
    - a ready-to-use toolbox for building web apps faster and more easily
    - makes code cleaner and more oraganized
    - handles common tasks (like routing, error handling, etc.)
- React: frontend library
    - favorite frontend library
- Node: JavaScript runtime
    - allows you to run JS on server

full-stack app
- client (frontend) sends request to server (backend) and gets a response back
- API (application programming interface) allows two difference apps to talk to each other
- REST API: uses HTTP methods (GET, POST, PUT, DELETE)
- HTTP status codes
    - 1xx: informational
    - 2xx: success (200:OK, 201:created)
    - 3xx: redirection
    - 4xx: client errors (400:bad request, 401:unauthorized, 403:forbidden, 404:not found, 429:too many requests)
    - 5xx: server errors (500:internal server error, 503:service unavailable)
- endpoint: a combination of a URL + HTTP method that lets the client interact with a specific resource
- middleware: a function that runs in the middle between the request and the response
    - useful for auth check & rate limiting

Databases
- SQL
    - structured data (data stored in tables like spreadsheet)
    - uses SQL language
    - best for complex queries
- NO-SQL
    - flexible data format (data stored like JSON or key-value pairs)
    - uses Query langauge or API
    - best for big data & real-time apps

Middleware
- a function that runs in the middle between the request and the response (useful for auth check & rate limiting)
- rate limiting: a way to control how often someone can do something on a website or app
    - e.g. how many times they can refresh a page, make a request to an API, or try to log in
    - e.g. only 100 requests every 15 minutes 
    - prevents abuse
    - protects servers from getting overwhelmed

For dev
- npm run dev (preview of website)
- npm install nodemon -D (tracks changes without rerunning)
- dotenv package allows you to keep secrets separate from the codebase

CORS (Cross-Origin Resource Sharing)
- a browser security rule
- when a website tries to get data from another website, the browser might block it for security reasons


external apps used:
- MongoDB: database
- Postman: testing API
- upstash (Redis): rate limiting

libraries used:
- react-hot-toast: notification
- tailwind css (v3.4.17 with Vite): css
- daisyUI (v4.12.24): themes that works with tailwind css

packages used:
- lucide-react
- axios
- cors


HOW TO DEPLOY
- push code to github
    1. hide .env file using .gitignore
    2. git init > git add . > git commit -m "intitial commit"
    3. create new repo on github
    4. push an existing repo from the command line
- use render.com
    1. npm init -y (creates package.json file)
    2. under "scripts": install dependencies, run frontend, start backend
    3. combine domains & remove CORS in server.js
    4. make a new web server with free plan (goes inactive after 15min)
- live @ https://mern-thinkboard-zbqv.onrender.com/