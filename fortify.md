# [WIP] Fortify Local Scan

## Prerequisites
1. Ensure source code is compilable 
2. Access to Software Security Center

### Required Environment Variables
**`FORTIFY_BUILD_ID`** - REQUIRED\
Build Id to track files for translate and scan

**`SSC_URL`** - REQUIRED\
Fortify Software Security Center URL

**`SSC_TOKEN`** - REQUIRED\
Generate a CIToken from Fortify Software Security Center

**`SSC_APP_NAME`** - REQUIRED\
Application name in Fortify Software Security Center

**`SSC_APP_VER_NAME`** - REQUIRED\
Application Version name in Fortify Software Security Center

# Use Case
- Perform a SAST scan on a Java application
- Upload scan result to Software Security Center