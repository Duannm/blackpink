## Boilerplate:
### 1. Feature
- React native navigation
- Mobx
- i18next
- axios

Dev: 
- husky
- eslint (for both js and ts)
 "lint": "concurrently \"yarn type-check\" \"yarn tslint\" \"yarn prettier\" \"eslint .\""
- prettier
 "prettier": "prettier --check \"**/*.tsx\" \"**/*.ts\" \"**/*.js\"",
- semantic-release
- commmitlint
- type check, tslint
 "type-check": "tsc -p tsconfig.json --noEmit",
 "tslint": "tslint -p tsconfig.json -c tslint.json",

```
type(scope?): subject  #scope is optional; multiple scopes are supported (current delimiter options: "/", "\" and ",")

- build
- ci
- chore
- docs
- feat
- fix
- perf
- refactor
- revert
- style
- test

Example:
chore: run tests on travis ci
fix(server): send cors headers
feat(blog): add comment section

```
## Mobile development process
### 1. Init project
#### Input Requirement:
- Package name/ Bundle ID
- Project name
- App name
- Icon

#### Check requirement with:
- Using map: (google/mapbox)
- Using chart: (MPchart, SVG)
- Using notification: Setup firebase and config app information
- Update online, update rule: code push
- Using analytics/crash report: google
- IAP
- Deeplink for mobile.
- Other specific features.

### 2. Setup environment
#### Preparation:
- Prepare keystore android
- Prepare certification ios

#### Git flow: 
- Local / Dev (for testing) -> branch: develop
- STG (for customer) -> branch: stg
- Production (for end-user) -> branch: master
- Production with feature: -> branch: version

- Android: using flavor
- IOS: using schema

#### Setup CI/CD:
##### - CI:
+ static check: eslint with rule, prettier
+ validate convention, check error language (JS)
+ validate test ID for component testing

##### - CD:
+ Android: build and upload to server google testing
+ IOS: using testflight, build with fastlane

### 3. Develop feature
- Rule when develop
- Structure project
- Best practice with new JS feature: clean, performance, readable code, sharing code in team (code of conduct).

### 4. Publish App
- Security
- Policy of store: 
 + Android
 + IOS
 
- Requirement: 
 + Description
 + Short description
 + Screenshot
 + Feature image
 + Category
 + Rating content

### 5. Monitor, Operation, Maintain App.