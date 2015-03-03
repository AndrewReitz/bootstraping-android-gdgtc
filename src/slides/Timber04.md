## Timber

Use it!

```
class ExampleActivity extends Activity {
  @Override protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.example_activity);
    Timber.d("Activity Created");

    try { ... } catch(Exception e) {
      Timber.e(e, "Something blew up");
    }
    ...
    Timber.i("Myobject is %s", myobject);
    Timber.tag("pieces029");
    Timber.d("look over here!");
  }
}
```

Output:
`ExampleActivity` // TODO

