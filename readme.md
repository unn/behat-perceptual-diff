# unn/behat-perceptual-diff

## What's going on here?

When you run the tests, the driver takes a screenshot and compares it to the baseline found in the pdiffs folder.

## How to get the most out of this demo?

Run through the instructions below, then after you think this is awesome, add your own features. You'll need to run them twice, once to establish a baseline and a second time to do the diff-ing.

## Alright, lets go!

### To run locally on your mac

Install selenium2 and imagemagick

```sh
brew install selenium-server-standalone imagemagick
```

Start selenium2

```sh
selenium-server -p 4444 &
```

Grab composer dependencies
```sh
composer update
```

Run the tests (will likely fail)

```sh
./vendor/bin/behat --format=pretty,html --out=,report.html
```
