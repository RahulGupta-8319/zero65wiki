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
