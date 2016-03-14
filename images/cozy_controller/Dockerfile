FROM node:4

MAINTAINER Simon Constans "simon@constans.io"

# install npm dependencies
RUN npm install -g coffee-script \
 && npm install -g cozy-controller \
 && npm install -g cozy-monitor

# install apt-get dependencies
RUN apt-get update --quiet \
 && apt-get install --quiet --yes \
  git

COPY ./docker-entrypoint.sh /
RUN chmod +x /docker-entrypoint.sh

#ENTRYPOINT ["/docker-entrypoint.sh"]

EXPOSE 9002

CMD ["cozy-controller"]
