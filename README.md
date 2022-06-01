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
* __Machine:__ Linux fv-az129-948 5.13.0-1023-azure #27~20.04.1-Ubuntu SMP Mon Apr 25 22:39:07 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Wed Jun  1 01:07:09 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.0  | ✓      | 66602.8    | 14.53   | 11.88         |
| bare                     | 10.13.0 | ✗      | 65378.8    | 14.80   | 11.66         |
| 0http                    | 3.3.0   | ✓      | 65177.6    | 14.84   | 11.62         |
| polkadot                 | 1.0.0   | ✗      | 65055.2    | 14.88   | 11.60         |
| foxify                   | 0.10.20 | ✓      | 64668.8    | 14.99   | 10.61         |
| connect                  | 3.7.0   | ✗      | 63509.6    | 15.25   | 11.33         |
| rayo                     | 1.3.10  | ✓      | 62374.4    | 15.53   | 11.12         |
| polka                    | 0.5.2   | ✓      | 62167.2    | 15.59   | 11.09         |
| micro                    | 9.3.4   | ✗      | 61713.6    | 15.70   | 11.01         |
| yeps                     | 1.1.1   | ✗      | 58869.6    | 16.49   | 10.50         |
| server-base              | 7.1.32  | ✗      | 58570.4    | 16.57   | 10.45         |
| micro-route              | 2.5.0   | ✓      | 58262.4    | 16.67   | 10.39         |
| restana                  | 4.9.5   | ✓      | 57759.2    | 16.81   | 10.30         |
| server-base-router       | 6.1.5   | ✓      | 56564.8    | 17.18   | 10.09         |
| connect-router           | 1.3.7   | ✓      | 55142.4    | 17.64   | 9.83          |
| trek-router              | 1.2.0   | ✓      | 54568.0    | 17.84   | 8.95          |
| trek-engine              | 1.0.5   | ✗      | 51804.0    | 18.81   | 8.50          |
| yeps-router              | 1.2.0   | ✓      | 47883.2    | 20.39   | 8.54          |
| vapr                     | 0.5.5   | ✓      | 46823.2    | 20.86   | 7.68          |
| koa                      | 2.13.4  | ✗      | 43921.6    | 22.27   | 7.83          |
| spirit                   | 0.6.1   | ✗      | 43596.0    | 22.45   | 7.77          |
| spirit-router            | 0.5.0   | ✓      | 43337.6    | 22.59   | 7.73          |
| total.js                 | 3.4.13  | ✓      | 42481.6    | 23.03   | 13.00         |
| restify                  | 8.6.1   | ✓      | 40327.4    | 24.32   | 7.27          |
| koa-router               | 10.1.1  | ✓      | 38518.2    | 25.46   | 6.87          |
| hapi                     | 20.2.2  | ✓      | 33289.0    | 29.54   | 5.94          |
| microrouter              | 3.1.3   | ✓      | 32032.0    | 30.71   | 5.71          |
| egg.js                   | 2.35.0  | ✓      | 18747.6    | 52.82   | 6.60          |
| express                  | 4.18.1  | ✓      | 13139.2    | 75.56   | 2.34          |
| express-with-middlewares | 4.18.1  | ✓      | 11278.0    | 88.11   | 4.32          |
| express-route-prefix     | 4.18.1  | ✓      | 10809.4    | 91.94   | 4.00          |
| fastify-big-json         | 3.29.0  | ✓      | 10546.2    | 94.27   | 121.33        |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
