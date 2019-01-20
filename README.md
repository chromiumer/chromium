### To Use Chromium browser Sync Service.

#### step one.
```
mv /Applications/Chromium.app/Contents/MacOS/Chromium /Applications/Chromium.app/Contents/MacOS/Chromium_bin
```

#### step two.
```
cat <<EOF>> /Applications/Chromium.app/Contents/MacOS/Chromium
#!/bin/bash

# Set up environment variables
export GOOGLE_API_KEY="xxx"
export GOOGLE_DEFAULT_CLIENT_ID="yyy"
export GOOGLE_DEFAULT_CLIENT_SECRET="zzz"

# Launch Chromium
/Applications/Chromium.app/Contents/MacOS/Chromium_bin
EOF
```
#### step three.
```
chmod +x /Applications/Chromium.app/Contents/MacOS/Chromium
```


>:christmas_tree:
https://console.developers.google.com 
To Get GOOGLE_API_KEY && GOOGLE_DEFAULT_CLIENT_ID && GOOGLE_DEFAULT_CLIENT_SECRET
