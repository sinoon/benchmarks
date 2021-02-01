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
* __Machine:__ Linux fv-az177-256 5.4.0-1036-azure #38~18.04.1-Ubuntu SMP Wed Jan 6 18:26:30 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.20.1`
* __Run:__ Mon Feb  1 01:39:00 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.11.0  | ✓      | 69641.2    | 13.88   | 12.42         |
| polkadot                 | 1.0.0   | ✗      | 68868.4    | 14.04   | 12.28         |
| bare                     | 10.13.0 | ✗      | 66667.6    | 14.51   | 11.89         |
| polka                    | 0.5.2   | ✓      | 66327.2    | 14.60   | 11.83         |
| 0http                    | 3.0.0   | ✓      | 65886.4    | 14.68   | 11.75         |
| connect                  | 3.7.0   | ✗      | 65221.6    | 14.85   | 11.63         |
| foxify                   | 0.10.20 | ✓      | 65182.4    | 14.86   | 10.69         |
| rayo                     | 1.3.6   | ✓      | 64936.0    | 14.92   | 11.58         |
| micro                    | 9.3.4   | ✗      | 64297.6    | 15.07   | 11.47         |
| server-base              | 7.1.23  | ✗      | 63677.6    | 15.21   | 11.36         |
| yeps                     | 1.1.1   | ✗      | 60682.4    | 15.99   | 10.82         |
| restana                  | 4.8.1   | ✓      | 60574.4    | 16.02   | 10.80         |
| server-base-router       | 6.1.5   | ✓      | 59262.4    | 16.37   | 10.57         |
| micro-route              | 2.5.0   | ✓      | 59063.2    | 16.43   | 10.53         |
| connect-router           | 1.3.5   | ✓      | 58591.2    | 16.57   | 10.45         |
| trek-engine              | 1.0.5   | ✗      | 56947.2    | 17.07   | 9.34          |
| trek-router              | 1.2.0   | ✓      | 56276.8    | 17.28   | 9.23          |
| yeps-router              | 1.2.0   | ✓      | 49540.0    | 19.68   | 8.83          |
| vapr                     | 0.5.5   | ✓      | 48732.0    | 20.02   | 7.99          |
| koa                      | 2.13.1  | ✗      | 47725.6    | 20.46   | 8.51          |
| spirit                   | 0.6.1   | ✗      | 45172.8    | 21.65   | 8.06          |
| spirit-router            | 0.5.0   | ✓      | 44132.8    | 22.17   | 7.87          |
| total.js                 | 3.4.7   | ✓      | 43632.0    | 22.43   | 13.36         |
| restify                  | 8.5.1   | ✓      | 42432.0    | 23.07   | 7.65          |
| koa-router               | 10.0.0  | ✓      | 42291.0    | 23.15   | 7.54          |
| hapi                     | 20.1.0  | ✓      | 34398.6    | 28.57   | 6.13          |
| microrouter              | 3.1.3   | ✓      | 32901.4    | 29.89   | 5.87          |
| egg.js                   | 2.29.1  | ✓      | 20067.3    | 49.31   | 7.06          |
| express                  | 4.17.1  | ✓      | 13430.0    | 73.91   | 2.39          |
| express-with-middlewares | 4.17.1  | ✓      | 11628.2    | 85.43   | 4.46          |
| express-route-prefix     | 4.17.1  | ✓      | 10988.6    | 90.46   | 4.07          |
| fastify-big-json         | 3.11.0  | ✓      | 10781.4    | 92.18   | 124.04        |
| farrow-http              | 1.5.3   | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
