# Places-API

This is an API containing data for all the cities of the World. It uses a **JSON file** as the database which is available at **[Datahub](https://datahub.io/core/world-cities#data)**

## Documentation

You can use ***places-api*** to fetch data and use it in your projects.

The data is extracted from [geonames](https://geonames.org), a very exhaustive list of worldwide toponyms.

### Fetching Method using Javascript will be Updated soon.
<br>

```json

//Data is passed as an Object from the JSON file to the Server

{
    "placesData": [
        {
            "country": "India",
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
<br>

This [datapackage](https://dataprotocols.org/data-packages/) only list cities above 15,000 inhabitants. Each city is associated with its country and subcountry to reduce the number of ambiguities. Subcountry can be the name of a state (eg in United Kingdom or the United States of America) or the major administrative section (eg ‘‘region’’ in France’’). See admin1 field on geonames website for further info about subcountry.


## Usage

- Open Gitbash/Terminal/Windows-Powershell

- Copy the following command to clone this repository in your local storage:
```
git clone https://github.com/pooranjoyb/places-api.git
```
- Hit the Enter key.

It would take a few seconds to clone the repository onto your system.<br>
Note: Please note that cloning depends on the internet connection and the time would depend on your connection bandwidth. If Git is not able to clone due to a weak connection, it would display a fatal error and the user is requested to try again until the above message does not appear.

- Check in the local drive by navigating to it manually.

- Run the following command to run the API

```
npm start
```

Contributions and Commits are apppreciated. 

## Dependencies

- Nodemon (v2.0.20)
- JSON-server (v0.17.1)

## Agreement

This data is provided "as is" without warranty or any representation of accuracy, timeliness or completeness.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.