## Timber

Setup

```
public class ExampleApp extends Application {
  @Override public void onCreate() {
    super.onCreate();

    if (BuildConfig.DEBUG) {
      Timber.plant(new DebugTree());
    } else {
      // Plant Custom Tree
    }
  }
}
```
