## Retrofit + RxJava

```
service.getListings("androiddev")
  .flatMap(new Func1<List<Listing>, Observable<Listing>() {
    @Override Object call(List<Listing> listings) {
      return Observable.from(listings);
    }
  }).flatMap(new Func1<Listing, Observable<List<Comments>>() {
    @Override Observable<List<Comment> call(Listing list) {
      return service.loadComments(list.getId)
    }
  }).flatMap(new Func1<List<Comment>, Observable<Comment>() {
    @Override Observable<Comment> call(List<Comment> comments) {
      return Observable.from(comments)
    }
  }).forEach(new Action1<Listing>() {
    @Override void call(Listing listing) {
      ...
  }
})
```