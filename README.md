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
* __Machine:__ Linux fv-az1152-750 6.8.0-1014-azure #16~22.04.1-Ubuntu SMP Thu Aug 15 21:31:41 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux | 4 vCPUs | 16GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.22.12`
* __Run:__ Tue Oct  1 01:11:26 UTC 2024

|                          | Version | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:     | --:    | :-:        | --:     | --:           |
| polkadot                 | 1.0.0   | ✗      | 78592.0    | 12.23   | 14.02         |
| fastify                  | 3.29.5  | ✓      | 68018.0    | 14.20   | 12.13         |
| bare                     | 10.13.0 | ✗      | 66033.2    | 14.65   | 11.78         |
| foxify                   | 0.10.20 | ✓      | 65342.4    | 14.81   | 10.72         |
| polka                    | 0.5.2   | ✓      | 63535.2    | 15.24   | 11.33         |
| connect                  | 3.7.0   | ✗      | 63358.8    | 15.28   | 11.30         |
| micro                    | 9.4.1   | ✗      | 60308.8    | 16.08   | 10.76         |
| yeps                     | 1.1.1   | ✗      | 60176.0    | 16.12   | 10.73         |
| server-base              | 7.1.32  | ✗      | 60116.0    | 16.14   | 10.72         |
| connect-router           | 1.3.8   | ✓      | 57337.6    | 16.94   | 10.23         |
| server-base-router       | 6.1.5   | ✓      | 56113.6    | 17.32   | 10.01         |
| trek-engine              | 1.0.5   | ✗      | 54460.0    | 17.86   | 8.93          |
| micro-route              | 2.5.0   | ✓      | 54456.0    | 17.86   | 9.71          |
| trek-router              | 1.2.0   | ✓      | 53388.8    | 18.23   | 8.76          |
| spirit                   | 0.6.1   | ✗      | 47894.4    | 20.41   | 8.54          |
| yeps-router              | 1.2.0   | ✓      | 47813.6    | 20.42   | 8.53          |
| vapr                     | 0.5.5   | ✓      | 47181.6    | 20.70   | 7.74          |
| spirit-router            | 0.5.0   | ✓      | 46468.8    | 20.99   | 8.29          |
| koa                      | 2.15.3  | ✗      | 46148.0    | 21.17   | 8.23          |
| total.js                 | 3.4.13  | ✓      | 42821.6    | 22.85   | 13.11         |
| restify                  | 8.6.1   | ✓      | 42508.8    | 23.03   | 7.66          |
| koa-router               | 10.1.1  | ✓      | 42048.8    | 23.28   | 7.50          |
| hapi                     | 20.3.0  | ✓      | 36527.4    | 26.87   | 6.51          |
| microrouter              | 3.1.3   | ✓      | 33962.4    | 28.94   | 6.06          |
| express                  | 4.21.0  | ✓      | 15030.4    | 66.00   | 2.68          |
| fastify-big-json         | 3.29.5  | ✓      | 13309.2    | 74.58   | 153.11        |
| express-with-middlewares | 4.21.0  | ✓      | 12608.8    | 78.76   | 4.83          |
| express-route-prefix     | 4.21.0  | ✓      | 11167.6    | 88.98   | 4.13          |
| 0http                    | 3.5.3   | ✓      | N/A        | N/A     | N/A           |
| egg.js                   | 2.37.0  | ✓      | N/A        | N/A     | N/A           |
| farrow-http              | 1.12.0  | ✗      | N/A        | N/A     | N/A           |
| rayo                     | 1.4.6   | ✓      | N/A        | N/A     | N/A           |
| restana                  | 4.9.9   | ✓      | N/A        | N/A     | N/A           |
| take-five                | 2.0.0   | ✓      | N/A        | N/A     | N/A           |
