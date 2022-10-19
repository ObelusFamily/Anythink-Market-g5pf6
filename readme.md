# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

To get your enviroment up and running first of ,you will have to install docker

[install docker](https://docs.docker.com/get-docker/)

Verify that docker is ready by running `docker -v` and `docker-compose -v`

You should see a response like this `Docker version 20.10.12, build e91ed57` and `docker-compose version 1.29.2, build 5becea4c`

Then, run `docker-compose up` from the project root directory to load Anythink's backend and frontend.

You can confirm that Docker is working correctly and that the backend is running and able to connect to your local database by pointing your browser to (http://localhost:3000/api/ping)

If after pointing your browser to (http://localhost:3000/api/ping), you see a response like, 

`ActiveRecord::PendingMigrationError`, just click on the *Rerun migrations* button on your browser page to resolve the pending migrations.