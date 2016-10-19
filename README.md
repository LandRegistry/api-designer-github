# api-designer-github
Version of mulesoft/api-designer which pulls files from Github

Very loosely based on https://github.com/stephanesan/api-designer, instead of implementing filesystem uses localStorage and populates from Github since this makes mocking work correctly.  Currently only supports flat file structure in github (no sub-directories), user can save but changes are lost when reloading the page.  Parameters are used to determine project to retrieve files from, e.g. 

http://rawgit.com/LandRegistry/api-designer-github/master/api-designer-github.html?gitApi=api.github.com/&gitRepo=LandRegistry/llc-api&gitPath=/application/static/schema&gitRef=develop

# Parameters
- gitApi - URI for github api to use (allows for corp github)
- gitRepo - Name of the repo containing raml
- gitPath - Directory within github repo which contains raml
- gitRef - Git reference to use for retrieval (i.e. branch, commit id, tag etc.)
