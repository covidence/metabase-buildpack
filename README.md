Heroku Buildpack for Metabase

Add the following to your app.json:

"buildpacks": [
  {
    "url": "https://github.com/metabase/metabase-buildpack"
  }
]

To set the version of metabase set the METABASE_VERSION environment variable in your heroku app.

e.g.

heroku config:set METABASE_VERSION=0.52.4 --app my-metabase-app