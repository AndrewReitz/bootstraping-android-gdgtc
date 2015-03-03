## Velcro

### Project Structure

```
${projectName}.gradle - main gradle file

src -+
     |
     +--debug - assests and sources ONLY in debug builds
     |
     +--main - assets and sources in ALL builds
     |
     +--release - assests and sources ONLY in release builds
```

Can easily switch logging, icons and strings based on build type.
See `${projectName}AppInitializer.java`
