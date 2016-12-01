FROM ubuntu:16.04

# TZ already set to UTC

# Set non interactive mode
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections

# populate apt cache of packages
RUN apt-get update

# upgrade any base dependancies
RUN apt-get upgrade -y

# Base packages we expect
RUN apt-get install -y build-essential python-software-properties libssl-dev libreadline-dev git-core curl
