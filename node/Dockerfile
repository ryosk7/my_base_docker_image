FROM ryosk7/mybase:debian-jessie
CMD ["bin/bash"]
RUN curl -SL https://deb.nodesource.com/setup_11.x | bash
RUN apt-get install -y nodejs
RUN npm install -g vue-cli
ENV HOST 0.0.0.0
EXPOSE 3000

