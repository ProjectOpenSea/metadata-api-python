## Python Metadata API for OpenSea Creatures

### About

This is a very simple sample Python Flask app for serving the ERC721 metadata for the [OpenSea creatures ERC721 contracts](https://github.com/ProjectOpenSea/opensea-creatures/), as specified in the [OpenSea developer docs](https://docs.opensea.io/docs/2-adding-metadata).

## Requirements

### Python 3
You'll need a machine with Python 3 installed.

### Google Cloud Storage
You'll need a Google Cloud Storage account with a project, bucket, and credentials.

## Setup

Create a .env file with the following:

```
export GOOGLE_STORAGE_PROJECT="<your_project>"
export GOOGLE_STORAGE_BUCKET="<your_bucket>"
```

Place your Google cloud storage credentials in a file called `credentials/google-storage-credentials.json`.

Create a virtualenv with Python3 and run `pip install -r requirements.txt`. 

## Running

Run the API with `python app.py` and hit http://localhost:5000/api/creature/1

## Deploying

To deploy on Heroku, set the `GOOGLE_STORAGE_PROJECT` and `GOOGLE_STORAGE_BUCKET` environment variables on your Heroku instance and deploy by pushing to your Heroku remote.
