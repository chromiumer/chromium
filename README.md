### To Use Chromium browser Sync Service.

#### :point_right: :one:
```
mv /Applications/Chromium.app/Contents/MacOS/Chromium /Applications/Chromium.app/Contents/MacOS/Chromium_bin
```

#### :point_right: :two:
```
cat <<EOF>> /Applications/Chromium.app/Contents/MacOS/Chromium
#!/bin/bash

# Set up environment variables
export GOOGLE_API_KEY="xxx"
export GOOGLE_DEFAULT_CLIENT_ID="yyy"
export GOOGLE_DEFAULT_CLIENT_SECRET="zzz"

# Launch Chromium
/Applications/Chromium.app/Contents/MacOS/Chromium_bin --force-dark-mode
EOF
```
#### :point_right: :three:
```
chmod +x /Applications/Chromium.app/Contents/MacOS/Chromium
```

:clap:
:point_down:

```
https://console.developers.google.com 
To Get GOOGLE_API_KEY && GOOGLE_DEFAULT_CLIENT_ID && GOOGLE_DEFAULT_CLIENT_SECRET
```
