# cptv-download

This tool supports bulk downloading of thermal video recordings in
CPTV and MP4 format from a Cacophony API instance. Videos are grouped
into directories by the tagged animal type. Recordings are downloaded
in parallel.

# cptv-upload

This tool supports bulk uploading of thermal video recordings into a 
Cacophony API instance.  This is useful for setting up a development
server.   

## Installation

These tools require Python 3.5 or later.

* Create a virtualenv using your preferred method.
* Install dependencies: `pip install -r requirements.txt`
* Run with: `./cptv-download` or `./cptv-upload`

## Configuration

Use `--help` to see how to configure program.

## Queries

By default the most recent 100 recordings accessible to the user
account are queried but `API.query()` does support a number of
filtering options. The API server supports arbitrary queries so feel
free to extend `API.query()` if required.
