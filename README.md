// server.js
const express = require('express');
const bodyParser = require('body-parser');
const app = express();
const PORT = process.env.PORT || 5000;

app.use(bodyParser.json());

let items = [];

app.get('/items', (req, res) => {
  res.json(items);
});

app.post('/items', (req, res) => {
  const newItem = req.body;
  items.push(newItem);
  res.status(201).send('Item added successfully');
});

app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});

// App.js
import React, { useState, useEffect } from 'react';
import axios from 'axios';

function App() {
  const [items, setItems] = useState([]);

  useEffect(() => {
    axios.get('/items')
      .then(response => {
        setItems(response.data);
      })
      .catch(error => {
        console.error('Error fetching data: ', error);
      });
  }, []);

  return (
    <div>
      <h1>Restaurant Items</h1>
      <ul>
        {items.map(item => (
          <li key={item.id}>{item.name} - ${item.price}</li>
        ))}
      </ul>
    </div>
  );
}

export default App;

--->
