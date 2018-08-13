# isomorphic-apm

Isomorphic Apm api, for the browser and node.js

## UPDATE LOG

- v1.0.0 

## Getting Started

- `npm set registry http://gitlab.esf.fangdd.net:61627`
- `npm install @fdd/isomorphic-apm`


## Features

- apm isomorphic

## Keywords

- apm
- elastic-apm-node
- elastic-apm-js-base

## Example

```
import apm from '@fdd/isomorphic-apm';

const myApm = apm.start({
  // Set required app name (allowed characters: a-z, A-Z, 0-9, -, _, and space)
  serviceName: 'xxx',

  // Use if APM Server requires a token
  secretToken: '',

  // Set custom APM Server URL (default: http://localhost:8200)
  serverUrl: '',

  // Setting it to 0 will disable stack trace collection. Any finite integer
  // value will be used as the maximum number of frames to collect. Setting it
  // to Infinity means that all frames will be collected.
  // stackTraceLimit: 50,

  // The agent maintains an in-memory queue to which recorded transactions are
  // added when they end. The queue is flushed with regular intervals
  // controlled by the flushInterval config option.
  // Use the maxQueueSize option to force a flush of the queue when it reaches
  // a certain size (number of ended transactions) - even if the flushInterval
  // time isn’t reached yet.
  // Set to -1 to disable, in which case only flushInterval counts.
  // maxQueueSize: 20,
  // flushInterval: 5,

  active: true,
});
```


## License

[MIT License]
