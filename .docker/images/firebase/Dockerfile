FROM debian:buster

RUN apt-get update -qqy && apt-get install -qqy sudo curl
RUN curl -sL https://firebase.tools | bash
RUN SUDO_FORCE_REMOVE=yes apt-get remove -qqy sudo curl
