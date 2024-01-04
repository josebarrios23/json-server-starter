# Student Dashboard API

This server contains data about all of the current students in a cohort. You must build a dashboard for the instructor.

## Implementation

This server is created using the [`json-server`](https://www.npmjs.com/package/json-server) NPM package.

### Resources

The following resources exist:

- Students: `/api/students`


## Installation

1. Clone the repository.
1. `npm install`
1. `npm run dev`


## Returning Data

If you use the Destroy/Delete Function your data will be removed from the `db.json` file permanently.

To restore the data, 

1. Stop the server

1. Copy the data from `originalData.json` into `db.json`
