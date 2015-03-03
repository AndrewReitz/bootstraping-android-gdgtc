## RxJava/RxAndroid

### Sequences

```
Observable.from(Arrays.asList(1, 2, 3, 4, 5))
    .map(new Func1<Integer, String>() {
      @Override public String call(Integer i) {
        return String.valueOf(i);
      }
    })
    .filter(new Func1<String, Boolean>() {
      @Override public Boolean call(String s) {
        return Integer.parseInt(s) % 2 == 0;
      }
    })
    .toList()
    .forEach(new Action1<List<String>>() {
      @Override public void call(List<String> strings) {
        System.out.println(strings);
      }
    });
```

Output `[2, 4]`
