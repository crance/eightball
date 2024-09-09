# [WIP] Fortify ScanCentral SAST (Remote Translate)

## Prerequisites
1. Ensure source code is compilable 
2. Access to Fortify Software Security Center
3. ScanCentral SAST Controller (client_auto_update is enabled to get latest Fortify_ScanCentral_Client\<version\>_x64.zip )
4. ScanCentral SAST Sensor(s)

### Required Environment Variables
**`SSC_URL`** - REQUIRED\
Fortify Software Security Center URL

**`SSC_TOKEN`** - REQUIRED\
Generate a CIToken from Fortify Software Security Center

**`CLIENT_AUTH_TOKEN`** - REQUIRED\
`client_auth_token` setting in ScanCentral SAST Controller's config.properties

**`SSC_APP_NAME`** - REQUIRED\
Application name in Fortify Software Security Center

**`SSC_APP_VER_NAME`** - REQUIRED\
Application Version name in Fortify Software Security Center

# Use Case
- Perform a SAST scan on a Java application
- Use ScanCentral SAST to offload translation and scanning phases of code analysis to ScanCentral SAST Sensors
- Use ScanCentral SAST to automatically detect build tools (`-bt none` in this scenario)