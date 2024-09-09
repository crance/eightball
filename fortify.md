# [WIP] Fortify Remote Scan

## Prerequisites
1. Ensure source code is compilable 
2. Access to Software Security Center
3. ScanCentral SAST Controller (client_auto_update is enabled to get latest Fortify_ScanCentral_Client\<version\>_x64.zip )
4. ScanCentral SAST Sensor(s) are available

### Required Environment Variables
**`FORTIFY_BUILD_ID`** - REQUIRED\
Build Id to track files for translate and scan

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
- Perform local translate
- Use ScanCentral SAST to offload scanning phases of code analysis to ScanCentral SAST Sensors