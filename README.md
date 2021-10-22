[![Newman Tests](https://github.com/qaprisciladearaujo/newmanCiCd/actions/workflows/blank.yml/badge.svg?branch=main)](https://github.com/qaprisciladearaujo/newmanCiCd/actions/workflows/blank.yml)

### API automation using Postman + newman 

Repo for inlustrate how is possible automated test for API using Postman with newman 

### Framewokrs & Libs
- [SpaceX API](https://api.spacex.land/graphql/)
- [Postman](https://www.postman.com/downloads/)
- [Newman](https://www.npmjs.com/package/newman)
- [newman-reporter-htmlextra](https://www.npmjs.com/package/newman-reporter-htmlextra)

### How run 

- local test

```
  newman run ./collection/SpaceX.postman_collection.json -e ./environment/SpaceX.postman_environment.json
```


- with `newman-html-report`

```
    newman run ./collection/SpaceX.postman_collection.json -e ./environment/SpaceX.postman_environment.json -r htmlextra,cli --reporter-htmlextra-export ./testResults/htmlreport.html
```
