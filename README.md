# MERN Stack custom template

<img src="./design/mern.jpeg"></img>

**I use this repository as a starter template for my own projects.**
**Feel free to use it on your own.**

## Features

- Backend: (based on [create-express-api](https://www.npmjs.com/package/create-express-api) by [w3CJ](https://github.com/w3cj) 🙏🏻)
  - Cors
  - Dotenv
  - Express
  - Helmet
  - Morgan
- Frontend: (based on [create-react-app](https://github.com/facebook/create-react-app) by Facebook 🤙)
  - CRA Rewired, Less, babel-plugins (necessary for Antd)
  - Ant Design with custom config

## Usage

```bash
# Clone repository
git clone https://github.com/nicolas-racchi/mern-template.git
cd mern-template

# Install all dependencies both for client, server and wrapper folder.
cd client && npm install && cd ../server && npm install && cd .. && npm install
```

Then, connect your mongoDB database:
inside the `server` folder, create a file called `.env` and add the mongo connectionstring.

```bash
# Example (./server/.env)
NODE_ENV=development
DATABASE_URL=my_mongo_connection_string
```

A `.env.sample` file is provided in the server folder so you always know what are the required environment variables.

```bash
# Run client & server concurrently
npm run dev
```

## Other useful things

- **Locales**: Ant design support language locales. As default, this template uses en_US (english). To change this setting to your own language, open `client/index.js` and change en_US to your own language based on locale tags (find some of them [here](https://www.oracle.com/java/technologies/javase/jdk8-jre8-suported-locales.html#util-text))
