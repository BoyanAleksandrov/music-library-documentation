# Music Library Documentation

## Introduction

Welcome to the Music Library documentation! This front-end application (SPA) is designed for creating and managing music albums. Whether you're a music enthusiast looking to explore new albums or an artist wanting to share your work with the world, Music Library has you covered.

## Features
![Screenshot 2024-02-23 111dasdsa256](https://github.com/BoyanAleksandrov/music-library-documentation/assets/80381466/2dcadfb9-1f23-4a18-8310-d80a21db8a75)


### Browse Albums Catalog
- Visitors can easily browse through the extensive catalog of albums.
- Discover new music and explore various genres with ease.

### User Registration
- Users have the option to register with an email and password.
- Registration enables users to create their own album cards and personalize their experience.

### Create Album Cards
- Registered users can create their own album cards to showcase their music or favorite albums.
- Add album details, cover art, and other relevant information to share with the community.

### Edit and Delete Publications
- Album authors have full control over their publications.
- Easily edit album details or delete publications as needed to keep the catalog up to date.

## Getting Started

To get started with Music Library, follow these simple steps:



1. **Clone the Repository**: Clone the Music Library repository to your local machine.
   ```sh
   git clone https://github.com/your-username/music-library.git
2. **Install the dependencies**: If missing you should install the package.json dependencies by     typing the following in the terminal:
   ```sh
      npm install npm
   ```
   ![Screenshot adsdas-02-23 113227](https://github.com/BoyanAleksandrov/music-library-documentation/assets/80381466/fb1fb845-6566-43fb-a467-35a8e56ab265)

3. **Start the app**: To start the application you simply need to open the terminal and type       the following:
   ```sh
   npm start
   ```
   The server should start on **http://localhost:3000/** if the port isn't already in use!

## Test the application

Before running any **tests**, we should make sure a **web server** is started, and the application can be found at the **root** of its **network address**.

To make sure we have done that please reffer to the previous step that explains **how to run the application**!

**To execute the tests**:
1. Open the **terminal** (make sure not to close the terminal that is running the web server instance)
2. Run the **tests**:
   ```sh
   npm run test
You should get the following **output** in the **terminal**:

![Screenshot 2024-02ss-23 114535](https://github.com/BoyanAleksandrov/music-library-documentation/assets/80381466/79ff74a4-d332-45ff-b777-aa61d5a473f6)


## RESTful API

When you start the app **locally**, you can access the **API** documentation on: **http://localhost:3300/api-docs**

The following endpoints are available:

> GET /data/albums?sortBy=_createdOn%20desc
- List all albums
> GET /data/albums/{id}
- Returns an album by given **id**
> POST /data/albums
- Create a new album with the according **JSON object** in the **request body**:
  "singer","album","imageUrl","release","label","sales"
> PUT /data/albums/{id}
- Edit album by **id** (Using the same syntax of the JSON object in the request body)
> DELETE /data/albums/{id}
- Delete an album by **id**
> POST /users/login
- log an existing **user**
- send a JSON Object as following: "username","password"
> POST /users/register
- Registers a new user
- JSON Object: "email", "password"
> GET /users/logout
- Logs out an existing user
> POST /data/likes
- adds a like to an album
- Expects a **request body** with {albumId}

![d](https://github.com/BoyanAleksandrov/music-library-documentation/assets/80381466/c62f9d38-396f-45c1-9415-b50f24364c09)


![GitHub repo size](https://img.shields.io/github/repo-size/BoyanAleksandrov/music-library-documentation)
