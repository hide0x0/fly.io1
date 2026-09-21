# Take by me — Fly.io

This is a minimal Flask app that displays:

    Take by me

## Deploy

1. Install Fly CLI:

    curl -L https://fly.io/install.sh | sh

2. Log in:

    fly auth login

3. Enter this directory and run:

    ./deploy.sh

The configured Fly.io app name is `take-by-me`, so the expected URL is:

    https://take-by-me.fly.dev

If that app name is unavailable, edit `app = "take-by-me"` in `fly.toml` and the app name in `deploy.sh` to another unique name.

You can also deploy manually:

    fly apps create take-by-me
    fly deploy
