# Places-API

This is a NodeJS API containing data for all the Cities of the World. It uses a **JSON file** as the database which is available at **[Datahub](https://datahub.io/core/world-cities#data)**

## Documentation

You can use ***places-API*** to fetch data and use it in your projects.

The data is extracted from [geonames](https://geonames.org), a very exhaustive list of worldwide toponyms.

## Using the Fetch API

The Fetch API provides a JavaScript interface for accessing and manipulating parts of the protocol, such as requests and responses. It also provides a global fetch() method that provides an easy, logical way to fetch resources asynchronously across the network.

<br>

```js

fetch("https://places-api-q5mi.onrender.com/placesData")
.then(response => response.json())
.then(response => {
    response.forEach(data => {
        console.log(JSON.stringify(data, null, 2));
    });
})

```

    NOTE that the API will return an Array of Object hence JSON.stringify() method is used.


The following JSON file is available in the **/placesData** endpoint of the API

<br>

```json
{
    "placesData": [
        {
            "country": "India",""
            "geonameid": 1275339,
            "name": "Mumbai",
            "subcountry": "Maharashtra"
        },
        {
            "country": "India",
            "geonameid": 1261481,
            "name": "New Delhi",
            "subcountry": "NCT"
        },
        ...
    ]
}
```
    Data is served as an Array of Object from the server to the HTTP request
<br>

This [datapackage](https://dataprotocols.org/data-packages/) only list cities above 15,000 inhabitants. Each city is associated with its country and subcountry to reduce the number of ambiguities. Subcountry can be the name of a state (eg in United Kingdom or the United States of America) or the major administrative section (eg ‘‘region’’ in France’’).

## Usage

- Open Gitbash/Terminal/Windows-Powershell

- Copy the following command to clone this repository in your local storage:
```
git clone https://github.com/pooranjoyb/places-API.git
```
- Hit the Enter key.

It would take a few seconds to clone the repository onto your system.<br>
**Note:** Cloning depends on the internet connection and the time would depend on your connection bandwidth. If Git is not able to clone due to a weak connection, it would display a fatal error and the user is requested to try again until the above message does not appear.

- Check in the local drive by navigating to it manually.

- Run the following command to run the development server

```js
npm start
```

## Contribution

Contributions and Commits are apppreciated. <br> 
**ADD** your own city and create a **PULL REQUEST** to contribute 

## Dependencies

- Nodemon (v2.0.20)
- JSON-server (v0.17.1)

## Agreement

This data is provided "as is" without warranty or any representation of accuracy, timeliness or completeness.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

