# CCIILLC.com

## Login System

### Setup

1. Install dependencies:
   ```sh
   npm install express body-parser
   ```
const express = require('express');
const bodyParser = require('body-parser');

const app = express();
app.use(bodyParser.urlencoded({ extended: true }));

app.get('/', (req, res) => {
    res.send('Hello World');
});

app.listen(3000, () => {
    console.log('Server is running on port 3000');
});
node server.js