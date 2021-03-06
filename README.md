# MH_API_take_home 

## Goal
1) Complete server and database requirements - Done
2) Containerize applications and database - Done
3) Endpoint Testing - Incomplete

## Getting started

### Install Docker

1) Go to docker.com, then download and install Docker for your OS.

2) Run Docker Desktop

### Install dependencies

```shell
npm install
```

### Build the application container

```shell
npm run docker:build
```

### Build the database container

```shell
npm run docker:build_db
```

### Run the containers

```shell
npm run docker:start
```


### Examples
#### To test the API, copy the following url to Chrome or Safari 

#### 1) Get a list of programs
```shell
www.localhost:3000/program
```

#### 2) Get a list of sections for program_id: 1
```shell
www.localhost:3000/section/?&programId=1
```

#### 3) Get a list of activities for section_id: 1
```shell
www.localhost:3000/activities/?&sectionId=1
```

## Tests

supertest.js is functional, however, I did not have enough time to debug running it in the container environment. Nevertheless, these are the steps:

### Build the test container

```shell
npm run docker:build_test
```

### Build the test database container

```shell
npm run docker:build_db_test
```

### Run the test

```shell
npm run docker:test
```

## API Reference

Please refer to model.jpg for API reference and data models

#   N e i l s o n _ T a k e h o m e  
 