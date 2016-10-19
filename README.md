# api-designer-github
Version of mulesoft/api-designer which pulls files from Github

Very loosely based on https://github.com/stephanesan/api-designer, instead of implementing filesystem uses localStorage and populates from Github.  Currently only supports flat file structure, user can save but changes are lost when reloading the page.  Parameters are used to determine project to retrieve files from, e.g. 
```
<URL OF PAGE>?gitApi=api.github.com/&gitRepo=LandRegistry/llc-api&gitPath=/application/static/schema&gitRef=develop
```
