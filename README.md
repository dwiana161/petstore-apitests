# petstore-apitests (Postman)

This repository contains a Postman collection and environment for testing APIs using Newman version 6.2.1.

The collection and environment are stored in this repo, so you can run tests directly from GitHub.

---
## Clone the Repository

First, clone this repository to your local machine:
```
git clone https://github.com/dwiana161/petstore-apitests.git
```

## Prerequisites

Make sure your system has:

- [Node.js] (v14+)
- [npm]
- [Newman]

Second, open the folder in VSCode.
Third, Make sure to add the rabbit.jpeg image file to your local project folder before running any tests. And Copy the full image path of the file.


Install Newman globally:
```
npm install -g newman
```

## Run Locally
```
newman run SwaggerAPI.postman_collection.json -e env.json
```

## To generate HTML reports, also install:
```
npm install -g newman-reporter-html
```

## Generate HTML report
```
newman run SwaggerAPI.postman_collection.json -e env.json --reporters cli,html --reporter-html-export newman-report.html
```

## Run directly from GitHub
```
newman run https://raw.githubusercontent.com/dwiana161/petstore-apitests/refs/heads/main/SwaggerAPI.postman_collection.json -e env.json
```


