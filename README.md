This is an app to query whether your service dependencies are available, over time.

Go is used because it is self-contained. No dependencies to add. 
Just run this script from a server.

   curl ...

Bring up the UI. Specify the URLs to monitor and you'll see how consistently your URLs respond to calls.

Sequence of mvp:

0. Ping URL (or make HTTP request to URL alone) on the schedule specified.
0. A file of specify URLs or IPs, how often to ping, and keywords.
0. Web page to specify URLs or IPs and how often to ping.

0. Store response data in a time-series database (InfluxDB).
0. Web page to display line chart with anomalies.
0. Web page to list anomaly dates and times (paged)

0. Add GraphQL API to respond with the status and speed of servers under watch based on a keyword defined.

0. Add analytics (Machine Learning) to identify patterns, such as "don't plan on using this URL Fridays at 3pm because the system has been consistently down then".

0. Respond to GraphQL API query with best time.

Join me on this!
Money made from this project will be split according to line counts by each committer.
