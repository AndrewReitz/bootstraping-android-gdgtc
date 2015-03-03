## Icepick

```
class ExampleActivity extends Activity {
  @Icicle String username; // This will be automatically saved and restored

  @Override public void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    Icepick.restoreInstanceState(this, savedInstanceState);
  }

  @Override public void onSaveInstanceState(Bundle outState) {
    super.onSaveInstanceState(outState);
    Icepick.saveInstanceState(this, outState);
  }
}
```

* Just stuff in a BaseActivity/BaseFragment
* Works with everyting `Bundle` supports
