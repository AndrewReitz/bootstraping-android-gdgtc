## Hugo

```
@DebugLog
public class ExampleActivity extends Activity {
  @Override protected void onCreate(Bundle savedInstanceState) { ... }
  @Override protected void onResume() { ... }
}
```

Output:

 ``` 
 V/ExampleActivity: ⇢ onCreate(savedInstanceState="android.os.Bundle@12345f")
 V/ExampleActivity: ⇠ onCreate [16ms]
 V/ExampleActivity: ⇠ onResume
 V/ExampleActivity: ⇠ onResume [20ms]
 ```
