## Getting Started

First, run the development server:

```bash
/** @type {import('next').NextConfig} */
const cron = require('node-cron');

cron.schedule('* * * * *', function () {
  console.log('Say scheduled hello')
});

const nextConfig = {
  reactStrictMode: true,
}

module.exports = nextConfig
```