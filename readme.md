# Television Shows API

This server contains data about both movies and television shows on Hulu.

## Implementation

This server is created using the [`json-server`](https://www.npmjs.com/package/json-server) NPM package.

Some of the data came from [this Kaggle dataset.](https://www.kaggle.com/shivamb/hulu-movies-and-tv-shows)

### Resources

The following resources exist:

- Movies: `/api/movies`
- Shows: `/api/shows`

## Installation

1. Clone the repository.
1. `npm install`
1. `npm run dev`


## Returning Data

If you use the Destory/Delete Function your data will be removed from the `db.json` file permanently.

To restore the data, 

1. Stop the server

1. Copy the data from `originalData.json` into `db.json`
