<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparison table with percentage values based on fastest result; `benchmark compare -p`
# Benchmarks
* __Machine:__ Linux runnervmkj6or 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Feb  1 01:27:38 UTC 2026

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 74790.0    | 12.88   | 13.34         |
| fastify                  | 3.29.5  | ✓      | 68909.2    | 14.01   | 12.29         |
| bare                     | 10.13.0 | ✗      | 65833.2    | 14.70   | 11.74         |
| foxify                   | 0.10.20 | ✓      | 65256.4    | 14.83   | 10.71         |
| polka                    | 0.5.2   | ✓      | 62604.0    | 15.47   | 11.16         |
| connect                  | 3.7.0   | ✗      | 62280.0    | 15.56   | 11.11         |
| micro                    | 9.4.1   | ✗      | 60813.6    | 15.95   | 10.85         |
| server-base              | 7.1.32  | ✗      | 60116.8    | 16.14   | 10.72         |
| yeps                     | 1.1.1   | ✗      | 58219.2    | 16.68   | 10.38         |
| server-base-router       | 6.1.5   | ✓      | 56264.8    | 17.28   | 10.03         |
| micro-route              | 2.5.0   | ✓      | 55617.6    | 17.48   | 9.92          |
| trek-engine              | 1.0.5   | ✗      | 55449.6    | 17.54   | 9.09          |
| connect-router           | 1.3.8   | ✓      | 54795.2    | 17.76   | 9.77          |
| trek-router              | 1.2.0   | ✓      | 54016.0    | 18.02   | 8.86          |
| yeps-router              | 1.2.0   | ✓      | 48142.4    | 20.27   | 8.59          |
| vapr                     | 0.5.5   | ✓      | 46984.0    | 20.79   | 7.71          |
| spirit                   | 0.6.1   | ✗      | 46708.8    | 20.91   | 8.33          |
| koa                      | 2.16.3  | ✗      | 45652.8    | 21.40   | 8.14          |
| spirit-router            | 0.5.0   | ✓      | 44892.8    | 21.76   | 8.01          |
| total.js                 | 3.4.13  | ✓      | 43328.0    | 22.58   | 13.26         |
| restify                  | 8.6.1   | ✓      | 42174.4    | 23.21   | 7.60          |
| koa-router               | 10.1.1  | ✓      | 40485.6    | 24.20   | 7.22          |
| hapi                     | 20.3.0  | ✓      | 35038.4    | 28.04   | 6.25          |
| microrouter              | 3.1.3   | ✓      | 33045.2    | 29.76   | 5.89          |
| express                  | 4.22.1  | ✓      | 14657.0    | 67.68   | 2.61          |
| fastify-big-json         | 3.29.5  | ✓      | 12749.6    | 77.89   | 146.68        |
| express-with-middlewares | 4.22.1  | ✓      | 12152.0    | 81.71   | 4.66          |
| express-route-prefix     | 4.22.1  | ✓      | 11037.4    | 90.04   | 4.08          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
