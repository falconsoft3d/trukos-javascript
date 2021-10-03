# Hello World Node y Express
```
const express = require('express');
const app = express();

app.get('/', (req, res)=>{
    res.send('Hello World')
});

app.listen(3000, ()=>{
    console.log('Server on port 3000')
})
```

# Correrlo
```
node index.js
```
