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
* __Machine:__ Linux pkrvmbietmlfzoi 6.11.0-1015-azure #15~24.04.1-Ubuntu SMP Thu May  1 02:52:08 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Tue Jul  1 01:17:54 UTC 2025

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 72701.2    | 13.26   | 12.97         |
| fastify                  | 3.29.5  | ✓      | 66569.6    | 14.52   | 11.87         |
| bare                     | 10.13.0 | ✗      | 65059.2    | 14.88   | 11.60         |
| polka                    | 0.5.2   | ✓      | 63088.0    | 15.35   | 11.25         |
| foxify                   | 0.10.20 | ✓      | 62607.2    | 15.47   | 10.27         |
| connect                  | 3.7.0   | ✗      | 62132.8    | 15.60   | 11.08         |
| micro                    | 9.4.1   | ✗      | 60488.0    | 16.04   | 10.79         |
| server-base              | 7.1.32  | ✗      | 59848.0    | 16.21   | 10.67         |
| yeps                     | 1.1.1   | ✗      | 58388.0    | 16.63   | 10.41         |
| server-base-router       | 6.1.5   | ✓      | 56392.8    | 17.24   | 10.06         |
| micro-route              | 2.5.0   | ✓      | 54956.8    | 17.69   | 9.80          |
| connect-router           | 1.3.8   | ✓      | 54908.8    | 17.71   | 9.79          |
| trek-engine              | 1.0.5   | ✗      | 53196.0    | 18.31   | 8.73          |
| trek-router              | 1.2.0   | ✓      | 52610.4    | 18.51   | 8.63          |
| spirit                   | 0.6.1   | ✗      | 47076.0    | 20.75   | 8.40          |
| yeps-router              | 1.2.0   | ✓      | 46901.6    | 20.82   | 8.36          |
| vapr                     | 0.5.5   | ✓      | 45857.6    | 21.31   | 7.52          |
| koa                      | 2.16.1  | ✗      | 44421.6    | 22.01   | 7.92          |
| spirit-router            | 0.5.0   | ✓      | 43964.0    | 22.24   | 7.84          |
| total.js                 | 3.4.13  | ✓      | 42510.4    | 23.02   | 13.01         |
| restify                  | 8.6.1   | ✓      | 41204.8    | 23.77   | 7.43          |
| koa-router               | 10.1.1  | ✓      | 41159.2    | 23.80   | 7.34          |
| hapi                     | 20.3.0  | ✓      | 35737.0    | 27.48   | 6.37          |
| microrouter              | 3.1.3   | ✓      | 32855.0    | 29.94   | 5.86          |
| express                  | 4.21.2  | ✓      | 13811.0    | 71.85   | 2.46          |
| fastify-big-json         | 3.29.5  | ✓      | 13097.0    | 75.79   | 150.67        |
| express-with-middlewares | 4.21.2  | ✓      | 12505.2    | 79.42   | 4.79          |
| express-route-prefix     | 4.21.2  | ✓      | 11163.8    | 88.99   | 4.13          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
