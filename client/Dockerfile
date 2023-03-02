FROM node:16
RUN npm init -y vite@latest test-app -- --template vanilla
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
## EXPOSE [Port you mentioned in the vite.config file]
EXPOSE 5173
CMD ["npm", "run", "dev",  "--", "--host", "0.0.0.0", "--port", "5173"]