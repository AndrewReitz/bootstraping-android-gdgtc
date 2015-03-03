## Android Preferences

```
SharedPreferences preferences = 
    PreferenceManager.getDefaultSharedPreferences(context);
BooleanPreference hasUserOpenAppBefore =
    new BooleanPreference(preferences, "SeenAppBefore");

if (hasUserOpenAppBefore.isSet()) { ... }
hasUserOpenAppBefore.set(true);
hasUserOpenAppBefore.delete();
```

* Boolean, Int, Float, String, StringSet, and Enum (be careful it uses ordinal values)
* Better with Dagger