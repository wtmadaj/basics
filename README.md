1. [Running Locally](#RunningLocally)
    - [Node](#Node)
    - [Flutter](#Flutter)
2. [References](#References)


# Running Locally
## Node
```bash
nodemon [jsfile]
```

to watch handlebar and js files (like .hbs):
```bash
nodemon [jsfile] -e js,hbs
```

If package.json has a start script:
```bash
npm run start [or other script name]
```

## Flutter
```bash
flutter run
```

Run an alternate file:
```bash
flutter run -t lib/otherFile.dart
```

Target a device with verbose logs:
```bash
flutter run -v -d macos run
```

See available (running) devices:
```bash
flutter devices
```

# References
Chat App: https://github.com/andrewjmead/node-course-v3-code
