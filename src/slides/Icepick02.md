## Icepick


```
class ExampleActivity extends Activity {
  private static final String USERNAME_KEY = "user_name"

  private final String username;

  @Override public void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    if (savedInstanceState != null) {
    	username = savedInstanceState.getString(USERNAME_KEY);
    }
  }

  @Override public void onSaveInstanceState(Bundle outState) {
    super.onSaveInstanceState(outState);
    savedInstanceState.putString(USERNAME_KEY, userName);
  }
}
```

Before