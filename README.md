# SilviaMoreno_S2_Assessment

node_modules:
It's unnecessary for them to be in the repository, but they must be installed to make this project work
 
Bonus:
1. About needing to avoid using directly our personal API key in a repository, I think that .gitignore(ing) it could be a good option. Will be stores but out of sight. Or even, could be a good suggestion to create a tempvariable for it!

2. Scripts to run the tests:
newman run api\collection\todoIst.json
newman run api\collection\todoIst.json -e api\envVariables\variables.json

Script to generate the report (this one can be pasted in "test" field in package.json):
newman run api\collection\todoIst.json -r htmlextra --reporter-htmlextra-export api\reports\APITestingReport.html