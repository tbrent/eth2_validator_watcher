# ETH2 Validator Watcher

## Validator Watcher - eth2_validator_watcher.py

This is a fork of the original watcher that posts to a slack channel instead of telegram. All you need to do to get your watcher working is edit the script to contain your validator indices (at the top of the file; you can have multiple) and then run the script with `SLACK_BOT_TOKEN` and `SLACK_CHANNEL` defined as env vars. Lastly, set up a cronjob to run every 15 minutes, which can be done by the following: 

```
  crontab -e
  (then in new window)
  */15 * * * * /abs/path/to/script
```

This is assuming you have already created a bot in slack, which isn't too hard to figure out.
