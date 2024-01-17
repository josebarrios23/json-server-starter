# JSON Server Starter

<img src="./server.jpg" alt="server" width="400" height="400">

As a Frontend Developer, you might want to have a project where you simply show off your Frontend skills (e.g. ReactJS Skills, CSS Skills, DOM Manipulation Skills). 

Maybe you choose to specialize as a Frontend Dev. 

You do not always have to take the time to create a Back End REST API and Node Server if this is your intention. 

This JSON Server can allow you to create data on your backend as if you are using a database. You will have the ability to run full CRUD (GET, POST, PUT/PATCH, DELETE)

## Implementation

This server is created using the [`json-server`](https://www.npmjs.com/package/json-server) NPM package.

### Resources

To create a resource you must first create data. Feel free to use ChatGPT or [Mockaroo](https://www.mockaroo.com/) or you can even hard code the data yourself. 

**NOTE: The data you create MUST be an array of objects.**

You will place your created data in the `data/db.json` file and into the `data/originalData.json` file. The array of objects should be given a `key` and placed in the JSON object in the `db.json` and `originalData.json` files. e.g

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

### Endpoint Created Automagically

When using this format in your JSON, this will create an api endpoint. The endpoint will be based on the key that you give your array of objects. In the above example the key is `students`. 

Your endpoing would be `/api/students`. If the key had been people, then your endpoint would have been `api/people`

JSON server does this for you automagically.

Test it by running your server, then going to the browser and entering in the URL address bar, `localhost:5001/api/<the key for your array>`

You should see the data you added render in the browser


## Installation

1. Clone the repository.
1. Add your data to the json files
1. `npm install`
1. `npm run dev`


## Returning Data

If you use the Destroy/Delete Function your data will be removed from the `db.json` file permanently.

To restore the data, 

1. Stop the server

1. Copy the data from `originalData.json` into `db.json`
