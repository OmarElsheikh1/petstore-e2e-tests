# Pet-Store_E2E-Scenario
Pet Store_E2E Scenario New Pet Registration,
This project involves using Postman to test the Pet Store API. I created a collection with seven API requests and ran them using Newman, a command-line collection runner for Postman. Below are the steps I followed to set up and execute the task.

------

## Setup Steps

#### 1. **Create the Collection**

I created a Postman collection named **Pet Store - Nawy Task**, which includes seven requests:

- **POST**: Add a new pet
- **GET**: Get the pet by ID
- **PUT**: Update an existing pet
- **GET**: Get the pet by ID again
- **DELETE**: Delete the pet by ID
- **GET**: Assert the pet is deleted successfully
- **GET**: Find pets by status

Here’s a visual representation of the collection:





------

#### 2. **Install Node.js**

Newman requires Node.js to run.
Download and install Node.js from [Node.js official website](https://nodejs.org/). NPM, which is included with Node.js, will be installed automatically.

------

#### 3. **Install Newman**

Run the following command to install Newman globally on your device:

```
npm install -g newman
```

Verify the installation by checking the Newman version:

```
newman -v
```

------

#### 4. **Run the Collection**

I used the following command to run the collection and environment variables:

```
newman run Nawy_collection.json -e Nawy_environment.json
```

This executes the requests in the collection using the provided environment variables.

------

#### 5. **Generate an HTML Report**

To make the test results more presentable, I installed the `newman-reporter-htmlextra` package globally:

```
npm install -g newman-reporter-htmlextra
```

Then, I ran the collection again with the `htmlextra` reporter to generate an HTML report:

```
newman run Nawy_collection.json -e Nawy_environment.json -r htmlextra
```

------

## Outputs

- A summary of the collection's execution is displayed in the terminal.
- An HTML report is generated, providing detailed results for each request in the collection.











![screencapture-file-D-Omar-ITI-current-ITI-Jobs-Nawy-newman-Pet-Store-Nawy-Task-2025-02-01-22-14-22-028-0-html-2025-02-02-00_27_13](https://github.com/user-attachments/assets/60ca5f61-5a83-49ef-a6af-08b95d771c07)
