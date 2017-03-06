Slack app for Voting on Stories and Tickets remotely and asynchronously.

## Usage

1. Install this app to your Slack team visiting http://asyncvoter.tk and pressing on the `Add to Slack` button.
2. Run a voting session on an issue launching the new `/vote issue` command in any channel.
3. Submit your vote pressing on any of the three difficulty buttons (Easy, Medium or Hard).
4. Finish and reveal the result of the voting session by pressing on the `Reveal` button. (We recommend to wait until you will receive 3 or more votes)

## Known Issues

- Votes cannot be reseted. But users can vote multiple times on the same issue.
- It supports parallel voting sessions in different channels only.

## Questions/feedback?

Create an issue in this repo, or contact https://agileventures.slack.com/messages/async_voter

## Requirements

- [Redis](https://redis.io/) v3.2.8 or later
- [Node](https://nodejs.org) v7.6.0 or later

## Development

1. Install dependencies `npm install`

2. Run tests `npm test`

3. Run the server `npm run dev`

You **need** to set up your own Slack **team** and Slack **app** to continue!

## Setting Up your own Slack team and app

- [Create a Slack Team](https://slack.com/create)
- [Create a Slack app](https://api.slack.com/apps?new_app=1)
- Install `ngrok` and run `ngrok http 4390` to expose your local server
- Enable `Slash Commands` in your Slack app with `https://<YOUR-NGROK-URL>/commands`
- Enable `Interactive Messages` in your Slack app with `https://<YOUR-NGROK-URL>/actions`
- Rename `.env.example` to `.env` and set your Slack app tokens there
- Go to <http://localhost:4390> and follow the instructions.

## References

- [Getting started with Slack apps](https://api.slack.com/slack-apps)
- [Using ngrok to develop locally for Slack](https://api.slack.com/tutorials/tunneling-with-ngrok)
