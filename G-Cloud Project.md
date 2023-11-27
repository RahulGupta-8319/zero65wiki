## General Development flow:
code -> testing -> pre-production -> production

## Zero65 development flow:
code -> github -> webhook -> gcloud config/service -> cloud build

# Key points related to project:
1. BE is ready
2. FE is needed
3. FE must have approve button at each step of development flow
4. storing config in database
5. allow user to add own config in database 
6. checking of user added config
7. indian-stock-exchange is our test case for this project

# Zero65 cloud service key points:
1. config needs to be added for each service in build.json
2. it only decides what steps are requird, buiding work is done by cloud build
3. github push request using webhook everytime changes are done on github

## Pipeline Template

### For BE :   
- Commit -> build -> test cases -> Beta deployment -> manual approval -> gamma deployed -> manual approval -> prod deployment 
- build will get triggered with github webhook
- master branch cannot bypass test cases but other branches can
- beta deployment will by automatic
- gamma deployment will be after manual approval button trigger
- prod deployment will be after manual approval button trigger
    - Series: server1 -> approval -> server2 -> approval -> ....
    - parallel: server1 + server2 + server3 + ...
    - combination of both parallel and series
- Retry button will be given to latest log in master branch with option to choose commit
- roll back log will have some different log nomenclature
 
### For FE :
- commit -> beta -> gamma -> prod
