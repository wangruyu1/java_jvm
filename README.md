Java Perversions
================

Various java-related perversions. Do not try this in production. Unless you absolutely have to, or just feel like it, in which case totally do!

labs-time
----------------
A tool that tries to empirically estimate the precision of the various time-killers available.

Usage:
```
cd labs/
gradle clean shadow
java -cp build/libs/labs-unspecified-shadow.jar ru.gvsmirnov.perv.labs.time.TimerPrecisionTest
```

Currently supported time killers are: ```Thread.sleep()```, ```Locksupport.parkNanos()```, ```BlackHole.consumeCPU()```, spinloops
