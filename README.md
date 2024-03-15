# url-shortner
Introduction
This application provides URL shortening functionality, allowing users to encode long URLs into shorter, more manageable links.

How to run

1.Setup Backend Service
Ensure Node.js is installed.
Install Nest CLI globally: npm i -g @nestjs/cli
Install dependencies for the backend service: npm install .

2.Test/Start Backend Service
Run backend service tests: npm run test
Start backend service: npm run start

3.Start Frontend Service
Navigate to the client directory: cd client
Install dependencies for the frontend service: npm install .
Start frontend service: npm run start

4.Run the Application with Docker Compose
Ensure Docker is installed.
Make sure ports 3000 and 3001 are available.
Run docker-compose build to build the Docker images.
Once the build is complete, run docker-compose up to start the application.

5.Access Swagger Documentation
To view Swagger documentation, go to: https://localhost:3001/doc

Documentation
List of APIs
1.GET /api
Returns a list of all encoded URLs.

2.PUT /api/encode
Encodes a given URL.

3.GET /api/{code}
Retrieves the encoded URL associated with the provided code.

4.GET /api/static/{code}
Retrieves the encoded URL associated with the provided code.

5.GET /404
Provides statistics around accessed shortened URLs.

6.GET /{code}
Redirects encoded URL to the actual URL.

Limitations
 Challenges may arise in handling increased traffic and user load due to current architecture limitations. Implementing scaling strategies is crucial for maintaining smooth performance as the application grows.

Future Scope
 Develop browser extensions for seamless URL shortening directly from the browser toolbar.
