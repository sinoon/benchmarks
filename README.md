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
* __Machine:__ Linux fv-az252-37 5.13.0-1022-azure #26~20.04.1-Ubuntu SMP Thu Apr 7 19:42:45 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun May  1 01:09:54 UTC 2022

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.29.0  | ✓      | 58874.4    | 16.52   | 10.50         |
| bare                     | 10.13.0 | ✗      | 58529.6    | 16.60   | 10.44         |
| polkadot                 | 1.0.0   | ✗      | 57566.4    | 16.88   | 10.27         |
| 0http                    | 3.1.2   | ✓      | 56922.4    | 17.07   | 10.15         |
| rayo                     | 1.3.10  | ✓      | 55672.0    | 17.47   | 9.93          |
| foxify                   | 0.10.20 | ✓      | 55212.0    | 17.62   | 9.06          |
| micro                    | 9.3.4   | ✗      | 55145.6    | 17.64   | 9.84          |
| polka                    | 0.5.2   | ✓      | 55090.4    | 17.66   | 9.82          |
| connect                  | 3.7.0   | ✗      | 54011.2    | 18.03   | 9.63          |
| server-base              | 7.1.32  | ✗      | 53876.8    | 18.07   | 9.61          |
| yeps                     | 1.1.1   | ✗      | 51856.0    | 18.79   | 9.25          |
| server-base-router       | 6.1.5   | ✓      | 51268.0    | 19.01   | 9.14          |
| restana                  | 4.9.4   | ✓      | 51043.2    | 19.10   | 9.10          |
| connect-router           | 1.3.7   | ✓      | 50951.2    | 19.13   | 9.09          |
| micro-route              | 2.5.0   | ✓      | 50393.6    | 19.35   | 8.99          |
| trek-engine              | 1.0.5   | ✗      | 49032.0    | 19.90   | 8.04          |
| trek-router              | 1.2.0   | ✓      | 46558.4    | 20.98   | 7.64          |
| vapr                     | 0.5.5   | ✓      | 41935.2    | 23.35   | 6.88          |
| yeps-router              | 1.2.0   | ✓      | 41200.8    | 23.77   | 7.35          |
| koa                      | 2.13.4  | ✗      | 40779.4    | 24.04   | 7.27          |
| spirit                   | 0.6.1   | ✗      | 40740.0    | 24.07   | 7.27          |
| spirit-router            | 0.5.0   | ✓      | 38269.6    | 25.64   | 6.82          |
| total.js                 | 3.4.13  | ✓      | 36813.0    | 26.66   | 11.27         |
| restify                  | 8.6.1   | ✓      | 35377.0    | 27.76   | 6.38          |
| koa-router               | 10.1.1  | ✓      | 35026.2    | 28.07   | 6.25          |
| hapi                     | 20.2.2  | ✓      | 29940.8    | 32.90   | 5.34          |
| microrouter              | 3.1.3   | ✓      | 28550.0    | 34.53   | 5.09          |
| egg.js                   | 2.35.0  | ✓      | 18821.7    | 52.62   | 6.62          |
| express                  | 4.18.1  | ✓      | 11404.2    | 87.12   | 2.03          |
| express-with-middlewares | 4.18.1  | ✓      | 9732.0     | 102.17  | 3.73          |
| express-route-prefix     | 4.18.1  | ✓      | 9616.4     | 103.43  | 3.56          |
| fastify-big-json         | 3.29.0  | ✓      | 9043.1     | 109.97  | 104.03        |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
