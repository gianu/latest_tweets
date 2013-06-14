This is a simple script that fetch the latest tweets from your timeline using the new 1.1 API.

## Motivation

The new 1.1 Twitter API only works with oauth, so you cannot fetch the latest tweets wihout sending the authorization header.

This is a bad news for someone who wants to fetch the latests tweets using pure javascript, without backend. So, my solution to this problem was to create a simple script that fetch periodically the tweets and pipe the result to a file (that I will read later from my JS).

## Configuration

First you need to create an app in [dev.twitter.com](http://dev.twitter.com)

With the app created,  only thing that you need to configure in the script are:

* **screen_name:** your twitter username (e.g.: gianu).
* **tweet_count:** the number of tweets you want to retrieve.
* **consumer_key:** the consumer key provided by the app created in twitter.
* **consumer_secret:** the consumer secret provided by the app created in twitter.
* **oauth_token:** the auth_token provided by the app created in twitter.
* **oauth_secret:** the auth_secret provided by the app created in twitter.

## Bugs and Improvements

Feel free to [report](https://github.com/gianu/latest_tweets/issues) any bug that you found or create PR with improvements!
