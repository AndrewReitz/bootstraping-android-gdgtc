## ButterKnife

```
class ExampleActivity extends Activity {
  private EditText username, password;

  @Override public void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.simple_activity);

    username = (EditText) findViewById(R.id.user);
    password = (EditText) findViewById(R.id.pass);

    findViewById(R.id.submit).setOnClickListener(new OnClickListener() {
      public void onClick(View v) {
      	...
      }
    });
    ...
}
```

Before
