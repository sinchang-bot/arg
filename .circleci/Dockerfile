FROM mhart/alpine-node:11.3.0
WORKDIR /src
COPY package.json ./
RUN npm i
COPY index.js test.js ./
RUN npm run test
CMD bash <(curl -s https://codecov.io/bash) -t 07c98da6-2717-4063-ab1d-a9fa4bdfd1da
