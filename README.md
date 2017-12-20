ensemble-transpose serves existing datasets in the format that
[Ensemble](https://github.com/mozilla/ensemble) expects.

## Development

1. Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)
2. Run `python3 -m venv env`
3. Run `source env/bin/activate`
4. Run `pip install -r requirements.txt`
5. Run `heroku local`

## Deployment

Submodules are only installed on Heroku when new code is manually pushed from
Git. Pushes completed using the "automatic deploy from GitHub" feature will not
trigger installation of submodules.

For that reason, manual pushes to Heroku are recommended.

https://devcenter.heroku.com/articles/git-submodules#git-submodules
