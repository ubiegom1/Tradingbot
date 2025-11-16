# Tradingbot
 const express = require('express');
const app = express();
const port = process.env.PORT || 3000;

// ✅ Health check route
app.get('/health', (req, res) => {
  res.send('Backend is healthy');
});

// Optional: root route
app.get('/', (req, res) => {
  res.send('Welcome to the trading signals backend');
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});
