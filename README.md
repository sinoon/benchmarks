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
* __Machine:__ Linux runnervmnay03 6.14.0-1017-azure #17~24.04.1-Ubuntu SMP Mon Dec  1 20:10:50 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Mar  1 01:26:59 UTC 2026

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 70930.0    | 13.60   | 12.65         |
| fastify                  | 3.29.5  | ✓      | 65058.4    | 14.88   | 11.60         |
| foxify                   | 0.10.20 | ✓      | 62462.4    | 15.51   | 10.25         |
| bare                     | 10.13.0 | ✗      | 62126.4    | 15.61   | 11.08         |
| polka                    | 0.5.2   | ✓      | 61796.8    | 15.68   | 11.02         |
| connect                  | 3.7.0   | ✗      | 59584.0    | 16.29   | 10.63         |
| micro                    | 9.4.1   | ✗      | 59144.0    | 16.41   | 10.55         |
| server-base              | 7.1.32  | ✗      | 57039.2    | 17.04   | 10.17         |
| yeps                     | 1.1.1   | ✗      | 56651.2    | 17.15   | 10.10         |
| server-base-router       | 6.1.5   | ✓      | 54800.8    | 17.75   | 9.77          |
| connect-router           | 1.3.8   | ✓      | 53380.0    | 18.24   | 9.52          |
| micro-route              | 2.5.0   | ✓      | 53136.8    | 18.32   | 9.48          |
| trek-engine              | 1.0.5   | ✗      | 52600.0    | 18.52   | 8.63          |
| trek-router              | 1.2.0   | ✓      | 51642.4    | 18.87   | 8.47          |
| yeps-router              | 1.2.0   | ✓      | 45324.8    | 21.56   | 8.08          |
| vapr                     | 0.5.5   | ✓      | 45281.6    | 21.59   | 7.43          |
| spirit                   | 0.6.1   | ✗      | 45252.0    | 21.61   | 8.07          |
| spirit-router            | 0.5.0   | ✓      | 44124.0    | 22.16   | 7.87          |
| koa                      | 2.16.4  | ✗      | 43502.4    | 22.49   | 7.76          |
| total.js                 | 3.4.13  | ✓      | 41846.4    | 23.40   | 12.81         |
| restify                  | 8.6.1   | ✓      | 40455.2    | 24.22   | 7.29          |
| koa-router               | 10.1.1  | ✓      | 39934.2    | 24.54   | 7.12          |
| hapi                     | 20.3.0  | ✓      | 34158.6    | 28.77   | 6.09          |
| microrouter              | 3.1.3   | ✓      | 32255.4    | 30.50   | 5.75          |
| express                  | 4.22.1  | ✓      | 13914.6    | 71.33   | 2.48          |
| fastify-big-json         | 3.29.5  | ✓      | 12731.4    | 77.98   | 146.46        |
| express-with-middlewares | 4.22.1  | ✓      | 12147.6    | 81.77   | 4.66          |
| express-route-prefix     | 4.22.1  | ✓      | 10770.0    | 92.26   | 3.98          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
