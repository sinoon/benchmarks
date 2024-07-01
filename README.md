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
* __Machine:__ Linux fv-az883-170 6.5.0-1022-azure #23~22.04.1-Ubuntu SMP Thu May  9 17:59:24 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Mon Jul  1 01:08:44 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 76958.8    | 12.49   | 13.72         |
| fastify                  | 3.29.5  | ✓      | 66891.6    | 14.46   | 11.93         |
| bare                     | 10.13.0 | ✗      | 66026.4    | 14.65   | 11.77         |
| foxify                   | 0.10.20 | ✓      | 65337.6    | 14.81   | 10.72         |
| connect                  | 3.7.0   | ✗      | 64413.6    | 15.03   | 11.49         |
| polka                    | 0.5.2   | ✓      | 64076.4    | 15.11   | 11.43         |
| micro                    | 9.4.1   | ✗      | 62364.8    | 15.54   | 11.12         |
| server-base              | 7.1.32  | ✗      | 60744.0    | 15.97   | 10.83         |
| yeps                     | 1.1.1   | ✗      | 59224.8    | 16.39   | 10.56         |
| connect-router           | 1.3.8   | ✓      | 57967.2    | 16.76   | 10.34         |
| micro-route              | 2.5.0   | ✓      | 56656.8    | 17.15   | 10.10         |
| server-base-router       | 6.1.5   | ✓      | 56277.6    | 17.27   | 10.04         |
| trek-engine              | 1.0.5   | ✗      | 55208.8    | 17.61   | 9.06          |
| trek-router              | 1.2.0   | ✓      | 54718.4    | 17.78   | 8.98          |
| yeps-router              | 1.2.0   | ✓      | 48618.4    | 20.07   | 8.67          |
| spirit                   | 0.6.1   | ✗      | 47149.6    | 20.69   | 8.41          |
| vapr                     | 0.5.5   | ✓      | 46555.2    | 20.98   | 7.64          |
| spirit-router            | 0.5.0   | ✓      | 46180.8    | 21.12   | 8.24          |
| koa                      | 2.15.3  | ✗      | 45821.6    | 21.33   | 8.17          |
| restify                  | 8.6.1   | ✓      | 43063.2    | 22.72   | 7.76          |
| total.js                 | 3.4.13  | ✓      | 42903.2    | 22.80   | 13.13         |
| koa-router               | 10.1.1  | ✓      | 41448.0    | 23.63   | 7.39          |
| hapi                     | 20.3.0  | ✓      | 36795.0    | 26.68   | 6.56          |
| microrouter              | 3.1.3   | ✓      | 34234.0    | 28.70   | 6.10          |
| express                  | 4.19.2  | ✓      | 15788.6    | 62.81   | 2.82          |
| fastify-big-json         | 3.29.5  | ✓      | 13233.0    | 75.00   | 152.23        |
| express-with-middlewares | 4.19.2  | ✓      | 12873.4    | 77.11   | 4.94          |
| express-route-prefix     | 4.19.2  | ✓      | 11345.0    | 87.58   | 4.20          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
