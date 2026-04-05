FROM node:alpine

WORKDIR /app

# Copy package files and install
COPY package.json package-lock.json* ./
RUN npm install

# Copy the rest of the application
COPY . .

# Expose port and run the server
ENV PORT=4001
EXPOSE 4001

CMD ["node", "index.js"]
