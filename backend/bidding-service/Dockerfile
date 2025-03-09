FROM node:18

WORKDIR /app

# Copy package files first for layer caching
COPY package*.json ./

RUN npm install

# Copy source code
COPY . .

EXPOSE 5001

CMD ["npm", "start"]