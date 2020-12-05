# ETH2 Validator Watcher

## Validator Watcher - eth2_validator_watcher.py

This is a fork of the original watcher that posts to slack instead of telegram. All you need to do to get your watcher working is edit the script to contain your validator indices (at the top of the file) and then run the script with `SLACK_BOT_TOKEN` and `SLACK_CHANNEL` defined. Lastly, set up a cronjob to run every 15 minutes.
