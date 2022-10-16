## Getting Started

I had the same problem. What you can do are scheduled tasks with the node-cron library. You have to put your task which you want to schedule in your next.config.js file like so:

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
