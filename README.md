example-monitor
==============

Example Monitor

Installing example-monitor
--------------

Install example-monitor globally so probes are available in your application, and custom views are discovered by node monitor.

  npm install -g example-monitor


Installing example-monitor Probes
--------------

example-monitor probes are placed in your application by including monitor and example-monitor in your package.json file:

    "dependencies": {
      "monitor": ">=0.6.0 <0.7.0",
      "example-monitor": ">=0.1.0 <0.2.0",
      ...

Then including them in your application startup:

    ...
    require('monitor').start();
    require('example-monitor');
    ...

Monitoring
--------------

Once running in your application, example-monitor can be viewed using the node monitor dashboard.

    npm install -g monitor-dashboard
    npm start monitor-dashboard

See [monitor-dashboard](http://lorenwest.github.io/monitor-dashboard) for more information about the node monitor dashboard.
