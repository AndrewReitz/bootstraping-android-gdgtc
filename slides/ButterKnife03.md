## ButterKnife

```
class ExampleActivity extends Activity {
  @InjectView(R.id.user) EditText username;
  @InjectView(R.id.pass) EditText password;

  @OnClick(R.id.submit) void submit() {
    ...
  }

  @Override public void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.simple_activity);
    ButterKnife.inject(this);

    ...
  }
}
```

Better!
(And that's not even all the awesomeness)
