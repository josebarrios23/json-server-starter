# JSON Server Starter

As a Frontend Developer, you do not always want to take the time to create a Back End REST API and Node Server. Maybe you want to show off your React Skills or your CSS Skills.

This JSON Server can allow you to create data on your backend as if you are using a database. You will have the ability to run full CRUD (GET, POST, PUT/PATCH, DELETE)

## Implementation

This server is created using the [`json-server`](https://www.npmjs.com/package/json-server) NPM package.

### Resources

To create a resource you must first create data. Feel free to use ChatGPT or Mockaroo or hard code the data yourself. The data must be an array of objects.

You will place this data in the `data/db.json` file and into the `data/originalData.json` file. The array of objects should be given a key and placed in the JSON object. e.g

```json
{
    "students": [
        {
            "id": "D8-hEWB",
            "names": {
                "preferredName": "Israel",
                "middleName": "Benjamin",
                "surname": "Rodriguez"
            }
        },
          {
            "id": "R3-FEWX",
            "names": {
                "preferredName": "Marcel",
                "middleName": "Poumeau",
                "surname": "Camus"
            }
        }
    ]
}

```

***NOTE:***
When using this format in your JSON, this will create an api endpoint. The endpoint will be based on the key that you give your array of objects. In the above example the key is `students`. 

Your endpoing would be `/api/students`. If the key had been people, then your endpoint would have been `api/people`

JSON server does this for you automagically.


## Installation

1. Clone the repository.
1. `npm install`
1. `npm run dev`


## Returning Data

If you use the Destroy/Delete Function your data will be removed from the `db.json` file permanently.

To restore the data, 

1. Stop the server

1. Copy the data from `originalData.json` into `db.json`
