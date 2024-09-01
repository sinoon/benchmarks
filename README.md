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
* __Machine:__ Linux fv-az887-117 6.5.0-1025-azure #26~22.04.1-Ubuntu SMP Thu Jul 11 22:33:04 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Sun Sep  1 01:11:50 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 64690.8    | 15.04   | 11.54         |
| bare                     | 10.13.0 | ✗      | 57268.8    | 16.98   | 10.21         |
| fastify                  | 3.29.5  | ✓      | 57008.8    | 17.06   | 10.17         |
| polka                    | 0.5.2   | ✓      | 56615.2    | 17.17   | 10.10         |
| server-base              | 7.1.32  | ✗      | 55481.6    | 17.53   | 9.89          |
| connect                  | 3.7.0   | ✗      | 54435.2    | 17.88   | 9.71          |
| micro                    | 9.4.1   | ✗      | 54174.4    | 17.97   | 9.66          |
| foxify                   | 0.10.20 | ✓      | 50850.4    | 19.18   | 8.34          |
| connect-router           | 1.3.8   | ✓      | 50048.0    | 19.49   | 8.93          |
| yeps                     | 1.1.1   | ✗      | 49769.6    | 19.59   | 8.88          |
| server-base-router       | 6.1.5   | ✓      | 49736.8    | 19.61   | 8.87          |
| micro-route              | 2.5.0   | ✓      | 49658.4    | 19.65   | 8.86          |
| trek-engine              | 1.0.5   | ✗      | 45268.0    | 21.59   | 7.43          |
| trek-router              | 1.2.0   | ✓      | 44528.0    | 21.96   | 7.30          |
| vapr                     | 0.5.5   | ✓      | 41836.8    | 23.41   | 6.86          |
| yeps-router              | 1.2.0   | ✓      | 41025.6    | 23.88   | 7.32          |
| spirit                   | 0.6.1   | ✗      | 40249.4    | 24.38   | 7.18          |
| koa                      | 2.15.3  | ✗      | 39977.6    | 24.53   | 7.13          |
| spirit-router            | 0.5.0   | ✓      | 38266.6    | 25.67   | 6.82          |
| total.js                 | 3.4.13  | ✓      | 37590.2    | 26.10   | 11.51         |
| restify                  | 8.6.1   | ✓      | 37427.2    | 26.23   | 6.75          |
| koa-router               | 10.1.1  | ✓      | 35389.4    | 27.77   | 6.31          |
| hapi                     | 20.3.0  | ✓      | 31164.2    | 31.58   | 5.56          |
| microrouter              | 3.1.3   | ✓      | 29206.8    | 33.74   | 5.21          |
| express                  | 4.19.2  | ✓      | 13663.0    | 72.65   | 2.44          |
| fastify-big-json         | 3.29.5  | ✓      | 12108.0    | 82.03   | 139.29        |
| express-with-middlewares | 4.19.2  | ✓      | 11217.4    | 88.62   | 4.30          |
| express-route-prefix     | 4.19.2  | ✓      | 10007.2    | 99.34   | 3.70          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
