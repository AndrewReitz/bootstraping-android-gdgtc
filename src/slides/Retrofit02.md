# Retrofit

```
public interface RedditService {
  @GET("/r/{subreddit}.json")
  List<Listing> getListings(@Path("subreddit") String subreddit);
}

RestAdapter restAdapter = new RestAdapter.Builder()
        .setEndpoint("http://reddit.com")
        .build();

RedditService service = restAdapter.create(RedditService);
```
