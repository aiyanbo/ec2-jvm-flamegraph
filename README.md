# ec2-jvm-flamegraph

# Install
fetched from [GitHub](https://github.com/aiyanbo/ec2-jvm-flamegraph)

```
git clone --recursive https://github.com/aiyanbo/ec2-jvm-flamegraph.git
cd ec2-java-flamegraph
./install
```

# Configure Java
Java needs to be running with the `-XX:+PreserveFramePointer` option, so that perf_events can perform frame pointer stack walks. As mentioned earlier, this can cost some performance, between 0 and 3% depending on the workload.

# Synopsis

```
./record 60
./flamegraph
```

# Ref

- [jmaps](https://github.com/brendangregg/Misc/blob/master/java/jmaps)
- [Java in Flames](http://techblog.netflix.com/2015/07/java-in-flames.html)
