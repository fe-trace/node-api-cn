
除显式同步的 API 之外，所有 zlib API 均使用 libuv 的线程池。 
这可能会在某些应用程序中产生意外的效果，例如性能不佳（可以通过调整[池的大小][pool size]来缓和）和/或无法恢复的灾难性内存碎片。

