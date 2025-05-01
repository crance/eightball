# [WIP] Fortify on Demand SAST

## Prerequisites
1. Ensure source code is compilable 
2. Access to Fortify on Demand

### Required Environment Variables
**`FOD_PORTAL_URL`** - REQUIRED\
Fortify on Demand Portal URL

**`FOD_API_URL`** - REQUIRED\
Fortify on Demand API URL

**`FOD_API_KEY`** - REQUIRED\
Generate a CIToken from Fortify Software Security Center

**`FOD_API_SECRET`** - REQUIRED\
Generate a CIToken from Fortify Software Security Center

**`FOD_RELEASE_ID`** - REQUIRED\
Application Release Id to upload payload and initiate scan

**`PACKAGE_OPTS`**  - Optional (Default: empty value)\
Specify additional packaging options, eg:\
`-oss`, 
`-bt mvn`, 
`-bt mvn -bf pom.xml`

**`FOD_UPLOADER_NOTES`** - Optional (Default: empty value)\
Notes about the scan

# Use Case
- Perform a SAST scan on a Java application
- Use ScanCentral SAST to package payload
- Use ScanCentral SAST to automatically detect build tools (`-bt none` in this scenario)
- Use FoDUpload to upload to Fortify on Demand