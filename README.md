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
* __Machine:__ Linux fv-az173-972 5.15.0-1023-azure #29-Ubuntu SMP Wed Oct 19 22:37:08 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Dec  1 01:09:02 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.4  | ✓      | 55338.4    | 17.58   | 9.87          |
| polkadot                 | 1.0.0   | ✗      | 55113.6    | 17.66   | 9.83          |
| bare                     | 10.13.0 | ✗      | 54764.0    | 17.77   | 9.77          |
| polka                    | 0.5.2   | ✓      | 54582.4    | 17.82   | 9.73          |
| 0http                    | 3.4.1   | ✓      | 53892.0    | 18.07   | 9.61          |
| connect                  | 3.7.0   | ✗      | 53679.2    | 18.13   | 9.57          |
| foxify                   | 0.10.20 | ✓      | 52571.2    | 18.53   | 8.62          |
| micro                    | 9.4.1   | ✗      | 51062.4    | 19.10   | 9.11          |
| yeps                     | 1.1.1   | ✗      | 49932.0    | 19.54   | 8.91          |
| server-base              | 7.1.32  | ✗      | 48636.8    | 20.06   | 8.67          |
| connect-router           | 1.3.7   | ✓      | 48590.4    | 20.08   | 8.67          |
| restana                  | 4.9.6   | ✓      | 47909.6    | 20.39   | 8.54          |
| server-base-router       | 6.1.5   | ✓      | 47477.6    | 20.57   | 8.47          |
| micro-route              | 2.5.0   | ✓      | 46084.8    | 21.21   | 8.22          |
| trek-router              | 1.2.0   | ✓      | 45464.8    | 21.51   | 7.46          |
| trek-engine              | 1.0.5   | ✗      | 44024.2    | 22.22   | 7.22          |
| yeps-router              | 1.2.0   | ✓      | 40088.8    | 24.45   | 7.15          |
| koa                      | 2.13.4  | ✗      | 39343.0    | 24.93   | 7.02          |
| vapr                     | 0.5.5   | ✓      | 39311.8    | 24.94   | 6.45          |
| spirit                   | 0.6.1   | ✗      | 36139.2    | 27.20   | 6.44          |
| total.js                 | 3.4.13  | ✓      | 36052.6    | 27.24   | 11.04         |
| spirit-router            | 0.5.0   | ✓      | 35743.6    | 27.48   | 6.37          |
| restify                  | 8.6.1   | ✓      | 34600.8    | 28.40   | 6.24          |
| koa-router               | 10.1.1  | ✓      | 33754.6    | 29.12   | 6.02          |
| hapi                     | 20.2.2  | ✓      | 29781.2    | 33.07   | 5.31          |
| microrouter              | 3.1.3   | ✓      | 27123.6    | 36.37   | 4.84          |
| egg.js                   | 2.37.0  | ✓      | 18013.6    | 54.98   | 6.34          |
| express                  | 4.18.2  | ✓      | 10979.4    | 90.53   | 1.96          |
| express-with-middlewares | 4.18.2  | ✓      | 9620.1     | 103.38  | 3.69          |
| express-route-prefix     | 4.18.2  | ✓      | 8816.6     | 112.75  | 3.26          |
| fastify-big-json         | 3.29.4  | ✓      | 8650.5     | 114.99  | 99.51         |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
