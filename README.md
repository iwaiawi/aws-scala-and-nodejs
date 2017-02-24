aws-scala-and-nodejs
============

aws-scala-and-nodejs is serverless framework template which have multi functions by Scala and Node.js.

Requirements
------------

* serverless framework
* sbt

Install
-----

Run install command:

```shell
sls install -u https://github.com/iwaiawi/aws-scala-and-nodejs
```

Usage
-----

Run compile with proguard and deploy:

```shell
cd functions/helloScala
sbt proguard:proguard

cd ../../
sls deploy -v

sls invoke -f helloScala -v
sls invoke -f helloNodejs -v
```
