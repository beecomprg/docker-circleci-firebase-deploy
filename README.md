# Introduction
A docker image based on alpine NodeJS docker hub image with added firebase-tools

# Use with circleci
- copy config.yml.sample over to .circleci/config.yml
- configure your circleci build
- set build environment variable FIREBASE_TOKEN to the token that you get by running ```firebase login:ci``` on your *local* station
- the script takes into account project aliases and you should configure them by running ```firebase use --add```

# Standalone usage
- pull the image from docker hub ```docker pull beecomprg/docker-circleci-firebase-deploy```