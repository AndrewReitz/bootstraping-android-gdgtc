## RxJava/RxAndroid

It doesn't matter.

```
getSomeString().subscribe(System.out::println) // Synchronous

getSomeString()
  .subscribeOn(Schedulers.io())
  .observeOn(AndroidSchedulers.mainThread())
  .subscribe(System.out::println) // Async
```
