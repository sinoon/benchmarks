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
* __Machine:__ Linux fv-az224-873 5.8.0-1039-azure #42~20.04.1-Ubuntu SMP Thu Jul 15 14:11:07 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.5`
* __Run:__ Wed Sep  1 01:46:03 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.20.2  | ✓      | 69486.8    | 13.91   | 12.39         |
| 0http                    | 3.1.1   | ✓      | 68095.6    | 14.20   | 12.14         |
| foxify                   | 0.10.20 | ✓      | 67099.2    | 14.40   | 11.01         |
| polkadot                 | 1.0.0   | ✗      | 67094.8    | 14.42   | 11.97         |
| bare                     | 10.13.0 | ✗      | 66581.2    | 14.51   | 11.87         |
| micro                    | 9.3.4   | ✗      | 66060.4    | 14.65   | 11.78         |
| polka                    | 0.5.2   | ✓      | 65666.4    | 14.72   | 11.71         |
| rayo                     | 1.3.6   | ✓      | 65217.6    | 14.85   | 11.63         |
| connect                  | 3.7.0   | ✗      | 62531.8    | 15.51   | 11.15         |
| yeps                     | 1.1.1   | ✗      | 61822.4    | 15.69   | 11.03         |
| server-base              | 7.1.29  | ✗      | 61304.8    | 15.82   | 10.93         |
| restana                  | 4.9.1   | ✓      | 60648.0    | 16.01   | 10.82         |
| micro-route              | 2.5.0   | ✓      | 60092.0    | 16.15   | 10.72         |
| server-base-router       | 6.1.5   | ✓      | 59506.4    | 16.31   | 10.61         |
| connect-router           | 1.3.5   | ✓      | 57049.6    | 17.04   | 10.17         |
| trek-router              | 1.2.0   | ✓      | 54331.2    | 17.92   | 8.91          |
| trek-engine              | 1.0.5   | ✗      | 53000.0    | 18.37   | 8.69          |
| vapr                     | 0.5.5   | ✓      | 47965.6    | 20.35   | 7.87          |
| yeps-router              | 1.2.0   | ✓      | 47735.2    | 20.45   | 8.51          |
| koa                      | 2.13.1  | ✗      | 46500.0    | 21.01   | 8.29          |
| spirit-router            | 0.5.0   | ✓      | 43865.6    | 22.32   | 7.82          |
| spirit                   | 0.6.1   | ✗      | 43696.0    | 22.40   | 7.79          |
| total.js                 | 3.4.10  | ✓      | 42767.2    | 22.88   | 13.09         |
| koa-router               | 10.1.1  | ✓      | 42316.6    | 23.14   | 7.55          |
| restify                  | 8.5.1   | ✓      | 42015.2    | 23.30   | 7.57          |
| hapi                     | 20.1.5  | ✓      | 34936.2    | 28.12   | 6.23          |
| microrouter              | 3.1.3   | ✓      | 32700.4    | 30.08   | 5.83          |
| egg.js                   | 2.30.0  | ✓      | 19977.5    | 49.54   | 7.03          |
| express                  | 4.17.1  | ✓      | 13345.8    | 74.38   | 2.38          |
| express-with-middlewares | 4.17.1  | ✓      | 11665.4    | 85.17   | 4.47          |
| express-route-prefix     | 4.17.1  | ✓      | 10383.2    | 95.72   | 3.84          |
| fastify-big-json         | 3.20.2  | ✓      | 3475.6     | 286.40  | 39.98         |
| farrow-http              | 1.10.9  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
