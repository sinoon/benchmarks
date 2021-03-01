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
* __Machine:__ Linux fv-az227-737 5.4.0-1039-azure #41~18.04.1-Ubuntu SMP Mon Jan 18 14:00:01 UTC 2021 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.20.2`
* __Run:__ Mon Mar  1 01:32:26 UTC 2021

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| fastify                  | 3.12.0  | ✓      | 69634.0    | 13.88   | 12.42         |
| polkadot                 | 1.0.0   | ✗      | 67133.2    | 14.40   | 11.97         |
| bare                     | 10.13.0 | ✗      | 65368.4    | 14.81   | 11.66         |
| foxify                   | 0.10.20 | ✓      | 65263.2    | 14.83   | 10.71         |
| micro                    | 9.3.4   | ✗      | 64527.6    | 15.00   | 11.51         |
| rayo                     | 1.3.6   | ✓      | 63764.8    | 15.19   | 11.37         |
| server-base              | 7.1.23  | ✗      | 63472.8    | 15.26   | 11.32         |
| 0http                    | 3.0.0   | ✓      | 63245.2    | 15.32   | 11.28         |
| connect                  | 3.7.0   | ✗      | 62146.4    | 15.59   | 11.08         |
| polka                    | 0.5.2   | ✓      | 61480.0    | 15.77   | 10.96         |
| yeps                     | 1.1.1   | ✗      | 61295.2    | 15.82   | 10.93         |
| connect-router           | 1.3.5   | ✓      | 60606.4    | 16.00   | 10.81         |
| server-base-router       | 6.1.5   | ✓      | 58878.4    | 16.49   | 10.50         |
| restana                  | 4.8.1   | ✓      | 58656.0    | 16.55   | 10.46         |
| micro-route              | 2.5.0   | ✓      | 57135.2    | 17.01   | 10.19         |
| trek-router              | 1.2.0   | ✓      | 54216.0    | 17.95   | 8.89          |
| trek-engine              | 1.0.5   | ✗      | 54057.6    | 18.00   | 8.87          |
| koa                      | 2.13.1  | ✗      | 49062.4    | 19.89   | 8.75          |
| vapr                     | 0.5.5   | ✓      | 48704.8    | 20.04   | 7.99          |
| yeps-router              | 1.2.0   | ✓      | 47573.6    | 20.52   | 8.48          |
| spirit                   | 0.6.1   | ✗      | 44264.8    | 22.10   | 7.89          |
| total.js                 | 3.4.8   | ✓      | 43251.2    | 22.63   | 13.24         |
| spirit-router            | 0.5.0   | ✓      | 42979.2    | 22.77   | 7.67          |
| koa-router               | 10.0.0  | ✓      | 42410.4    | 23.08   | 7.56          |
| restify                  | 8.5.1   | ✓      | 40707.2    | 24.06   | 7.34          |
| hapi                     | 20.1.0  | ✓      | 34339.0    | 28.62   | 6.12          |
| microrouter              | 3.1.3   | ✓      | 31226.0    | 31.52   | 5.57          |
| egg.js                   | 2.29.3  | ✓      | 19432.5    | 50.93   | 6.84          |
| express                  | 4.17.1  | ✓      | 12901.0    | 76.97   | 2.30          |
| express-with-middlewares | 4.17.1  | ✓      | 11199.2    | 88.74   | 4.29          |
| express-route-prefix     | 4.17.1  | ✓      | 10643.6    | 93.36   | 3.94          |
| fastify-big-json         | 3.12.0  | ✓      | 10370.8    | 95.85   | 119.31        |
| farrow-http              | 1.5.3   | ✗      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
