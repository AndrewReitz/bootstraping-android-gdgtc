## Retrofit + RxJava

```
public interface RedditService {
  @GET("/r/{subreddit}.json") Observable<Listing>
  getListings(@Path("subreddit") String subreddit);
}

service.getListings("androiddev").subscribe(new Action1<List<Listings>>() {
  @Override void call(List<Listings> listings) {
    ...
  }
})
```