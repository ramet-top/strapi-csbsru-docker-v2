FROM mhart/alpine-node:latest
# FROM mhart/alpine-node:10.8.0

ENV NODE_ENV=development
# ENV NODE_ENV=production

RUN mkdir -p /app
COPY . /app
WORKDIR /app

RUN yarn
RUN yarn run build
# RUN npm install
# RUN npm run build

ENV HOST 0.0.0.0
EXPOSE 3000
CMD ["yarn", "start"]


    
# FROM node:latest

# RUN mkdir /app
# WORKDIR /app

# COPY ./ /app/
# RUN npm install && npm run build

# ENV HOST 0.0.0.0
# EXPOSE 3000
# CMD ["strapi", "start"]