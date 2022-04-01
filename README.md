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
* __Machine:__ Linux fv-az133-970 5.11.0-1028-azure #31~20.04.2-Ubuntu SMP Tue Jan 18 08:46:15 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.10`
* __Run:__ Fri Apr  1 01:04:42 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.27.4  | ✓      | 64878.0    | 14.93   | 11.57         |
| polkadot                 | 1.0.0   | ✗      | 64394.0    | 15.05   | 11.48         |
| bare                     | 10.13.0 | ✗      | 62745.6    | 15.43   | 11.19         |
| 0http                    | 3.1.2   | ✓      | 62713.6    | 15.45   | 11.18         |
| foxify                   | 0.10.20 | ✓      | 62093.6    | 15.61   | 10.18         |
| polka                    | 0.5.2   | ✓      | 61851.2    | 15.66   | 11.03         |
| micro                    | 9.3.4   | ✗      | 61069.6    | 15.88   | 10.89         |
| connect                  | 3.7.0   | ✗      | 60999.2    | 15.89   | 10.88         |
| rayo                     | 1.3.10  | ✓      | 60533.6    | 16.03   | 10.80         |
| server-base              | 7.1.32  | ✗      | 58144.0    | 16.70   | 10.37         |
| restana                  | 4.9.3   | ✓      | 57215.2    | 17.01   | 10.20         |
| server-base-router       | 6.1.5   | ✓      | 56623.2    | 17.16   | 10.10         |
| yeps                     | 1.1.1   | ✗      | 56572.0    | 17.18   | 10.09         |
| connect-router           | 1.3.6   | ✓      | 56343.2    | 17.25   | 10.05         |
| micro-route              | 2.5.0   | ✓      | 55582.4    | 17.49   | 9.91          |
| trek-router              | 1.2.0   | ✓      | 53081.6    | 18.34   | 8.71          |
| trek-engine              | 1.0.5   | ✗      | 52440.0    | 18.58   | 8.60          |
| yeps-router              | 1.2.0   | ✓      | 46662.4    | 20.94   | 8.32          |
| koa                      | 2.13.4  | ✗      | 46152.8    | 21.16   | 8.23          |
| vapr                     | 0.5.5   | ✓      | 44156.8    | 22.16   | 7.24          |
| total.js                 | 3.4.13  | ✓      | 43073.6    | 22.71   | 13.19         |
| spirit                   | 0.6.1   | ✗      | 40915.2    | 23.95   | 7.30          |
| spirit-router            | 0.5.0   | ✓      | 39388.8    | 24.90   | 7.02          |
| koa-router               | 10.1.1  | ✓      | 39218.8    | 25.00   | 6.99          |
| restify                  | 8.6.1   | ✓      | 38983.2    | 25.15   | 7.03          |
| hapi                     | 20.2.1  | ✓      | 32499.6    | 30.27   | 5.80          |
| microrouter              | 3.1.3   | ✓      | 30908.0    | 31.85   | 5.51          |
| egg.js                   | 2.34.0  | ✓      | 19232.8    | 51.48   | 6.77          |
| express                  | 4.17.3  | ✓      | 13049.0    | 76.12   | 2.33          |
| express-with-middlewares | 4.17.3  | ✓      | 11403.6    | 87.12   | 4.37          |
| fastify-big-json         | 3.27.4  | ✓      | 10726.2    | 92.64   | 123.39        |
| express-route-prefix     | 4.17.3  | ✓      | 10606.2    | 93.74   | 3.92          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
