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
* __Machine:__ Linux fv-az93-436 5.8.0-1042-azure #45~20.04.1-Ubuntu SMP Wed Sep 15 14:24:15 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.7`
* __Run:__ Mon Nov  1 01:46:06 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| 0http                    | 3.1.1   | ✓      | 38213.8    | 25.68   | 6.81          |
| polkadot                 | 1.0.0   | ✗      | 36529.2    | 26.88   | 6.51          |
| fastify                  | 3.22.1  | ✓      | 36127.4    | 27.19   | 6.44          |
| bare                     | 10.13.0 | ✗      | 35862.2    | 27.39   | 6.40          |
| micro                    | 9.3.4   | ✗      | 35285.2    | 27.84   | 6.29          |
| rayo                     | 1.3.6   | ✓      | 34916.8    | 28.15   | 6.23          |
| polka                    | 0.5.2   | ✓      | 34651.4    | 28.35   | 6.18          |
| spirit                   | 0.6.1   | ✗      | 33393.0    | 29.54   | 5.96          |
| foxify                   | 0.10.20 | ✓      | 32767.6    | 30.03   | 5.37          |
| server-base              | 7.1.29  | ✗      | 31219.6    | 31.54   | 5.57          |
| restana                  | 4.9.1   | ✓      | 30788.4    | 31.99   | 5.49          |
| connect                  | 3.7.0   | ✗      | 30695.0    | 32.14   | 5.47          |
| yeps                     | 1.1.1   | ✗      | 30456.2    | 32.36   | 5.43          |
| trek-engine              | 1.0.5   | ✗      | 30313.3    | 32.51   | 4.97          |
| connect-router           | 1.3.5   | ✓      | 29720.4    | 33.16   | 5.30          |
| spirit-router            | 0.5.0   | ✓      | 29705.6    | 33.21   | 5.30          |
| server-base-router       | 6.1.5   | ✓      | 29061.6    | 33.90   | 5.18          |
| micro-route              | 2.5.0   | ✓      | 28143.2    | 35.04   | 5.02          |
| trek-router              | 1.2.0   | ✓      | 27556.0    | 35.81   | 4.52          |
| yeps-router              | 1.2.0   | ✓      | 26957.6    | 36.59   | 4.81          |
| vapr                     | 0.5.5   | ✓      | 24703.6    | 39.99   | 4.05          |
| koa                      | 2.13.4  | ✗      | 23887.3    | 41.36   | 4.26          |
| restify                  | 8.6.0   | ✓      | 22297.2    | 44.34   | 4.02          |
| total.js                 | 3.4.12  | ✓      | 21690.0    | 45.59   | 6.64          |
| koa-router               | 10.1.1  | ✓      | 21625.5    | 45.76   | 3.86          |
| microrouter              | 3.1.3   | ✓      | 18982.0    | 52.17   | 3.39          |
| hapi                     | 20.2.1  | ✓      | 18709.6    | 52.94   | 3.34          |
| egg.js                   | 2.31.0  | ✓      | 12667.4    | 78.42   | 4.46          |
| express                  | 4.17.1  | ✓      | 7756.1     | 128.38  | 1.38          |
| fastify-big-json         | 3.22.1  | ✓      | 7518.0     | 132.35  | 86.50         |
| express-route-prefix     | 4.17.1  | ✓      | 6720.1     | 148.04  | 2.49          |
| express-with-middlewares | 4.17.1  | ✓      | 6633.7     | 150.05  | 2.54          |
| farrow-http              | 1.10.9  | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
