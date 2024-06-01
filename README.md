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
* __Machine:__ Linux fv-az1118-881 6.5.0-1021-azure #22~22.04.1-Ubuntu SMP Tue Apr 30 16:08:18 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sat Jun  1 01:06:16 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 77126.4    | 12.47   | 13.75         |
| fastify                  | 3.29.5  | ✓      | 65989.2    | 14.66   | 11.77         |
| bare                     | 10.13.0 | ✗      | 63621.2    | 15.22   | 11.35         |
| foxify                   | 0.10.20 | ✓      | 63012.0    | 15.37   | 10.34         |
| polka                    | 0.5.2   | ✓      | 62437.6    | 15.52   | 11.13         |
| connect                  | 3.7.0   | ✗      | 60796.0    | 15.95   | 10.84         |
| micro                    | 9.4.1   | ✗      | 60463.2    | 16.04   | 10.78         |
| server-base              | 7.1.32  | ✗      | 59589.6    | 16.28   | 10.63         |
| yeps                     | 1.1.1   | ✗      | 57913.6    | 16.77   | 10.33         |
| server-base-router       | 6.1.5   | ✓      | 57002.4    | 17.04   | 10.17         |
| micro-route              | 2.5.0   | ✓      | 54825.6    | 17.74   | 9.78          |
| trek-engine              | 1.0.5   | ✗      | 54475.2    | 17.86   | 8.94          |
| connect-router           | 1.3.8   | ✓      | 53424.8    | 18.22   | 9.53          |
| trek-router              | 1.2.0   | ✓      | 53384.0    | 18.24   | 8.76          |
| yeps-router              | 1.2.0   | ✓      | 47220.0    | 20.68   | 8.42          |
| vapr                     | 0.5.5   | ✓      | 46080.8    | 21.20   | 7.56          |
| spirit-router            | 0.5.0   | ✓      | 45875.2    | 21.30   | 8.18          |
| spirit                   | 0.6.1   | ✗      | 45610.4    | 21.41   | 8.13          |
| koa                      | 2.15.3  | ✗      | 45298.4    | 21.58   | 8.08          |
| total.js                 | 3.4.13  | ✓      | 42421.6    | 23.07   | 12.99         |
| restify                  | 8.6.1   | ✓      | 42108.0    | 23.25   | 7.59          |
| koa-router               | 10.1.1  | ✓      | 41104.0    | 23.83   | 7.33          |
| hapi                     | 20.3.0  | ✓      | 36120.6    | 27.18   | 6.44          |
| microrouter              | 3.1.3   | ✓      | 33088.8    | 29.72   | 5.90          |
| express                  | 4.19.2  | ✓      | 14256.8    | 69.59   | 2.54          |
| fastify-big-json         | 3.29.5  | ✓      | 13162.8    | 75.42   | 151.44        |
| express-with-middlewares | 4.19.2  | ✓      | 12392.6    | 80.14   | 4.75          |
| express-route-prefix     | 4.19.2  | ✓      | 11204.8    | 88.67   | 4.15          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
