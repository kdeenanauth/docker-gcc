FROM kdeenanauth/gcc:1.0

MAINTAINER Kevin Deenanauth <kevin@deenanauth.com>

RUN mkdir -p /usr/src/app/source /usr/src/app/build
WORKDIR /usr/src/app/source

ONBUILD COPY . /usr/src/app/source
ONBUILD RUN g++ *.cpp -o /usr/src/app/build/output
ONBUILD WORKDIR /usr/src/app/build