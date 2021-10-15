{
  "version": "1.1.0",
  "vars": {
    "GIT_DOMAIN": "github.com",
    "SKIA_ROOT": "https://github.com/domchen/depsync/releases/download/1.0.1",
    "V8_ROOT": "https://github.com/domchen/depsync/releases/download/1.0.2"
  },
  "repos": {
    "common": [
      {
        "url": "https://${GIT_DOMAIN}/webmproject/libwebp.git",
        "commit": "1fe3162541ab2f5ce69aca2e2b593fab60520d34",
        "dir": "third_party/libwebp"
      },
      {
        "url": "https://${GIT_DOMAIN}/libjpeg-turbo/libjpeg-turbo.git",
        "commit": "129f0cb76346ceede8f4d8d87dea8acb0809056c",
        "dir": "third_party/libjpeg-turbo"
      }
    ]
  },
  "files": {
    "common": [
      {
        "url": "${SKIA_ROOT}/include.zip",
        "dir": "third_party/skia",
        "unzip": true
      },
      {
        "url": "${V8_ROOT}/include.zip",
        "dir": "third_party/v8",
        "unzip": "true"
      }
    ],
    "mac": [
      {
        "url": "${SKIA_ROOT}/darwin-x64.zip",
        "dir": "third_party/skia",
        "unzip": true
      },
      {
        "url": "${V8_ROOT}/darwin-x64.zip",
        "multipart": [
          ".001",
          ".002",
          ".003"
        ],
        "dir": "third_party/v8",
        "unzip": true
      }
    ],
    "win": [
      {
        "url": "${SKIA_ROOT}/win-ia32.zip",
        "dir": "third_party/skia",
        "unzip": true
      },
      {
        "url": "${V8_ROOT}/win-ia32.zip",
        "dir": "third_party/v8",
        "unzip": true
      }
    ]
  },
  "actions": {
    "common": [
      {
        "command": "npm install tspack",
        "dir": "./"
      },
      {
        "command": "node node_modules/tspack/bin/tspack --v",
        "dir": "./"
      }
    ]
  }
}