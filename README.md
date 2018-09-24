```
$ sbt publishLocal # ok
$ sbt publishLocalSigned
…
[error] java.lang.RuntimeException: Repository for publishing is not specified.
[error] 	at scala.sys.package$.error(package.scala:27)
[error] 	at sbt.Classpaths$.$anonfun$getPublishTo$1(Defaults.scala:2633)
[error] 	at scala.Option.getOrElse(Option.scala:121)
[error] 	at sbt.Classpaths$.getPublishTo(Defaults.scala:2633)
[error] 	at sbt.Classpaths$.$anonfun$ivyBaseSettings$48(Defaults.scala:2084)
[error] 	at scala.Function1.$anonfun$compose$1(Function1.scala:44)
[error] 	at sbt.internal.util.$tilde$greater.$anonfun$$u2219$1(TypeFunctions.scala:40)
[error] 	at sbt.std.Transform$$anon$4.work(System.scala:67)
[error] 	at sbt.Execute.$anonfun$submit$2(Execute.scala:269)
[error] 	at sbt.internal.util.ErrorHandling$.wideConvert(ErrorHandling.scala:16)
[error] 	at sbt.Execute.work(Execute.scala:278)
[error] 	at sbt.Execute.$anonfun$submit$1(Execute.scala:269)
[error] 	at sbt.ConcurrentRestrictions$$anon$4.$anonfun$submitValid$1(ConcurrentRestrictions.scala:178)
[error] 	at sbt.CompletionService$$anon$2.call(CompletionService.scala:37)
[error] 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
[error] 	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
[error] 	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
[error] 	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1142)
[error] 	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:617)
[error] 	at java.lang.Thread.run(Thread.java:745)
[error] (publishConfiguration) Repository for publishing is not specified.
…
```
