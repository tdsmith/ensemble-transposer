ensemble-transposer fetches raw data which has been generated by Mozilla data
engineers, adds metadata to it, and serves JSON with the data and metadata
combined. A related project, [Ensemble](https://github.com/mozilla/ensemble),
fetches this JSON and uses it to render dashboards.

The JSON that ensemble-transposer ingests follows a standard format
([example](http://fhwr-unflattener.herokuapp.com/)). The JSON that
ensemble-transposer generates and serves also follows a standard format
([example](http://ensemble-transposer.herokuapp.com/hardware/)). Because of
this, we can easily generate an Ensemble dashboard for any dataset that has been
[formatted properly](http://fhwr-unflattener.herokuapp.com/).

## Setup

Install [Docker CE](https://docs.docker.com/install/)

## Run

### For development

Run `npm run dev`

Any of the environment variables in *.env* can be overridden. For example: `PORT=1234 npm run dev`

### In production

Run `npm run prod`

Any of the environment variables in *.env* can be overridden. For example: `PORT=1234 npm run prod`

## Test

Run `npm test`
