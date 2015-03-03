# Retrofit

```
public interface RedditService {
  @GET("/r/{subreddit}.json")
  void getListings(@Path("subreddit") String subreddit, 
  Callback<List<Listing>> callback);
}

service.getListings("androiddev", new Callback() {
  @Override void success(List<Listing> listings, Response response) {
    ...
  }

  @Override void failure(RetrofitError error) {
    ...
  }
})
```
