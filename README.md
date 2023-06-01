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
* __Machine:__ Linux fv-az447-210 5.15.0-1037-azure #44-Ubuntu SMP Thu Apr 20 13:19:31 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Thu Jun  1 01:10:07 UTC 2023

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 68438.8    | 14.12   | 12.21         |
| fastify                  | 3.29.5  | ✓      | 66913.6    | 14.45   | 11.93         |
| 0http                    | 3.5.2   | ✓      | 66903.6    | 14.45   | 11.93         |
| bare                     | 10.13.0 | ✗      | 65782.4    | 14.71   | 11.73         |
| foxify                   | 0.10.20 | ✓      | 65655.6    | 14.74   | 10.77         |
| polka                    | 0.5.2   | ✓      | 65378.4    | 14.80   | 11.66         |
| server-base              | 7.1.32  | ✗      | 64621.6    | 14.98   | 11.52         |
| connect                  | 3.7.0   | ✗      | 63841.2    | 15.16   | 11.39         |
| yeps                     | 1.1.1   | ✗      | 63379.2    | 15.27   | 11.30         |
| restana                  | 4.9.7   | ✓      | 62644.0    | 15.49   | 11.17         |
| micro                    | 9.4.1   | ✗      | 61798.4    | 15.69   | 11.02         |
| server-base-router       | 6.1.5   | ✓      | 60108.8    | 16.14   | 10.72         |
| connect-router           | 1.3.8   | ✓      | 59315.2    | 16.36   | 10.58         |
| micro-route              | 2.5.0   | ✓      | 56395.2    | 17.24   | 10.06         |
| trek-router              | 1.2.0   | ✓      | 56318.4    | 17.26   | 9.24          |
| trek-engine              | 1.0.5   | ✗      | 56311.2    | 17.27   | 9.24          |
| vapr                     | 0.5.5   | ✓      | 51384.8    | 18.97   | 8.43          |
| yeps-router              | 1.2.0   | ✓      | 49908.8    | 19.53   | 8.90          |
| spirit-router            | 0.5.0   | ✓      | 46940.8    | 20.82   | 8.37          |
| koa                      | 2.14.2  | ✗      | 46675.8    | 20.92   | 8.32          |
| spirit                   | 0.6.1   | ✗      | 46668.0    | 20.94   | 8.32          |
| total.js                 | 3.4.13  | ✓      | 43824.0    | 22.32   | 13.42         |
| restify                  | 8.6.1   | ✓      | 43207.2    | 22.65   | 7.79          |
| koa-router               | 10.1.1  | ✓      | 40296.6    | 24.32   | 7.19          |
| hapi                     | 20.3.0  | ✓      | 34704.2    | 28.32   | 6.19          |
| microrouter              | 3.1.3   | ✓      | 33424.2    | 29.41   | 5.96          |
| express                  | 4.18.2  | ✓      | 14509.2    | 68.40   | 2.59          |
| express-with-middlewares | 4.18.2  | ✓      | 12349.2    | 80.45   | 4.73          |
| express-route-prefix     | 4.18.2  | ✓      | 12117.0    | 81.91   | 4.48          |
| fastify-big-json         | 3.29.5  | ✓      | 11117.4    | 89.36   | 127.90        |
| egg.js                   | 2.37.0  | ✓      | 8303.6     | 119.90  | 2.92          |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.0   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
