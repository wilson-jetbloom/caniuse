This is an app to query whether your service dependencies are available, over time.

Go is used because it is self-contained. No dependencies to add. 
Just run this script from a server.

   curl ...

Bring up the UI. Specify the URLs to monitor and you'll see how consistently your URLs respond to calls.

I hope to add analysis of patterns 
such as "don't plan on using this URL Fridays at 3pm because the system has been consistently down then".

Sequence of mvp:

1. Web page to specify URLs or IPs and how often to ping.
0. Ping URL or make HTTP request on the schedule specified.
0. Store data in a time-series database (InfluxDB).
0. Web page to display line chart with anomalies.
0. Web page to list anomaly dates and times.

0. Add analytics to identify patterns.

Join me on this!
