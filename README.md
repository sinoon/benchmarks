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
* __Machine:__ Linux fv-az90-725 5.11.0-1027-azure #30~20.04.1-Ubuntu SMP Wed Jan 12 20:56:50 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.9`
* __Run:__ Tue Feb  1 01:49:23 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 66980.4    | 14.45   | 11.95         |
| 0http                    | 3.1.1   | ✓      | 66294.8    | 14.59   | 11.82         |
| fastify                  | 3.27.0  | ✓      | 65709.6    | 14.73   | 11.72         |
| bare                     | 10.13.0 | ✗      | 65129.6    | 14.87   | 11.62         |
| rayo                     | 1.3.10  | ✓      | 64501.2    | 15.02   | 11.50         |
| polka                    | 0.5.2   | ✓      | 64253.2    | 15.07   | 11.46         |
| connect                  | 3.7.0   | ✗      | 62939.0    | 15.41   | 11.23         |
| foxify                   | 0.10.20 | ✓      | 62862.4    | 15.41   | 10.31         |
| server-base              | 7.1.29  | ✗      | 61519.2    | 15.76   | 10.97         |
| yeps                     | 1.1.1   | ✗      | 61180.8    | 15.86   | 10.91         |
| micro                    | 9.3.4   | ✗      | 60777.6    | 15.96   | 10.84         |
| restana                  | 4.9.2   | ✓      | 60361.6    | 16.06   | 10.76         |
| server-base-router       | 6.1.5   | ✓      | 58032.8    | 16.74   | 10.35         |
| micro-route              | 2.5.0   | ✓      | 57712.8    | 16.83   | 10.29         |
| connect-router           | 1.3.6   | ✓      | 56733.6    | 17.13   | 10.12         |
| trek-engine              | 1.0.5   | ✗      | 54936.8    | 17.71   | 9.01          |
| trek-router              | 1.2.0   | ✓      | 53530.4    | 18.18   | 8.78          |
| vapr                     | 0.5.5   | ✓      | 48376.8    | 20.17   | 7.94          |
| yeps-router              | 1.2.0   | ✓      | 47592.0    | 20.51   | 8.49          |
| koa                      | 2.13.4  | ✗      | 45470.4    | 21.50   | 8.11          |
| spirit                   | 0.6.1   | ✗      | 42789.6    | 22.88   | 7.63          |
| total.js                 | 3.4.13  | ✓      | 42471.2    | 23.05   | 13.00         |
| koa-router               | 10.1.1  | ✓      | 41420.0    | 23.65   | 7.39          |
| spirit-router            | 0.5.0   | ✓      | 41360.8    | 23.68   | 7.38          |
| restify                  | 8.6.0   | ✓      | 40847.2    | 23.98   | 7.36          |
| hapi                     | 20.2.1  | ✓      | 34330.2    | 28.63   | 6.12          |
| microrouter              | 3.1.3   | ✓      | 32744.2    | 30.04   | 5.84          |
| egg.js                   | 2.33.1  | ✓      | 21483.2    | 46.03   | 7.56          |
| express                  | 4.17.2  | ✓      | 14354.6    | 69.14   | 2.56          |
| express-with-middlewares | 4.17.2  | ✓      | 12679.8    | 78.31   | 4.86          |
| express-route-prefix     | 4.17.2  | ✓      | 12535.0    | 79.22   | 4.64          |
| fastify-big-json         | 3.27.0  | ✓      | 11900.2    | 83.48   | 136.90        |
| farrow-http              | 1.11.3  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
