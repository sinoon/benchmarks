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
* __Machine:__ Linux runnervmg1sw1 6.11.0-1018-azure #18~24.04.1-Ubuntu SMP Sat Jun 28 04:46:03 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Dec  1 01:19:59 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 71016.8    | 13.62   | 12.66         |
| fastify                  | 3.29.5  | ✓      | 64271.6    | 15.07   | 11.46         |
| bare                     | 10.13.0 | ✗      | 63227.2    | 15.32   | 11.28         |
| polka                    | 0.5.2   | ✓      | 61208.8    | 15.85   | 10.92         |
| foxify                   | 0.10.20 | ✓      | 60826.4    | 15.95   | 9.98          |
| connect                  | 3.7.0   | ✗      | 59854.4    | 16.22   | 10.68         |
| micro                    | 9.4.1   | ✗      | 58237.6    | 16.68   | 10.39         |
| server-base              | 7.1.32  | ✗      | 57709.6    | 16.84   | 10.29         |
| yeps                     | 1.1.1   | ✗      | 57154.4    | 17.00   | 10.19         |
| connect-router           | 1.3.8   | ✓      | 54344.8    | 17.91   | 9.69          |
| server-base-router       | 6.1.5   | ✓      | 54000.0    | 18.02   | 9.63          |
| micro-route              | 2.5.0   | ✓      | 53360.0    | 18.25   | 9.52          |
| trek-engine              | 1.0.5   | ✗      | 52267.2    | 18.64   | 8.57          |
| trek-router              | 1.2.0   | ✓      | 52120.8    | 18.69   | 8.55          |
| yeps-router              | 1.2.0   | ✓      | 46353.6    | 21.07   | 8.27          |
| vapr                     | 0.5.5   | ✓      | 45253.6    | 21.60   | 7.42          |
| koa                      | 2.16.3  | ✗      | 44797.6    | 21.83   | 7.99          |
| total.js                 | 3.4.13  | ✓      | 41992.8    | 23.31   | 12.85         |
| spirit-router            | 0.5.0   | ✓      | 41875.2    | 23.39   | 7.47          |
| spirit                   | 0.6.1   | ✗      | 41615.2    | 23.54   | 7.42          |
| restify                  | 8.6.1   | ✓      | 40493.6    | 24.20   | 7.30          |
| koa-router               | 10.1.1  | ✓      | 39040.2    | 25.12   | 6.96          |
| hapi                     | 20.3.0  | ✓      | 34237.8    | 28.71   | 6.11          |
| microrouter              | 3.1.3   | ✓      | 31756.0    | 30.99   | 5.66          |
| express                  | 4.21.2  | ✓      | 14167.8    | 70.06   | 2.53          |
| fastify-big-json         | 3.29.5  | ✓      | 12554.4    | 79.10   | 144.45        |
| express-with-middlewares | 4.21.2  | ✓      | 12118.0    | 81.96   | 4.65          |
| express-route-prefix     | 4.21.2  | ✓      | 11184.0    | 88.85   | 4.14          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
