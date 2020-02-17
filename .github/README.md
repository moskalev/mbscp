## mbscp – Multithreaded secure and efficient copying of block devices

A multithreaded version of [bscp](https://vog.github.io/bscp/) tool for high bandwidth high latency networks. Provides secure and efficient copying of block devices (and large files) between (very) distant machines.

### Use case and difference in architecture

I implemented mbscp to accomplish an intercontinental transfer of an hdd's image over the internet in a reasonable amount of time. While [bscp](https://vog.github.io/bscp/) works perfectly for not very distant machines, a high latency connection significantly hampers the transfer speed. mbscp uses multiple ssh connections to utilize high bandwidth connections in the presence of high latency.
