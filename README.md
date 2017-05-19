This is an app to query whether your service dependencies are available, over time.

Go is used because it is self-contained. No dependencies to add. 
Just run this script from a server.

   curl ...

Bring up the UI. Specify the URLs to monitor and you'll see how consistently your URLs respond to calls.

Sequence of mvp:

1. Ping URL (or make HTTP request to URL alone) on the schedule specified.
0. A file of specify URLs or IPs, how often to ping, and keywords.
0. Web page to specify URLs or IPs and how often to ping.
0. Web page has site feedback.

0. Store response data in a time-series database (InfluxDB).
0. Web page displays line chart with anomalies (Graphana).

   ![](https://cloud.githubusercontent.com/assets/243499/9864408/a7fff336-5b8c-11e5-8797-99494656a976.png)

0. Web page to list anomaly dates and times (paged).
0. Alert host down by sending email [via TICK Kapacitor]
0. Alert host down by sending SMS [via IFTTT?]. 
0. Add GraphQL API to respond with the status and speed of servers under watch based on a keyword defined.

0. Add analytics (Machine Learning) to identify patterns, such as "don't plan on using this URL Fridays at 3pm because the system has been consistently down then".

0. Respond to GraphQL API query with best time.

Join me on this!
Money made from this project will be split according to line counts by each committer.
