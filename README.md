# Anypoint Platform Development: Production-Ready Development Practices - DEX660

## Local Path
- PROJECT_HOME=/Users/yehan.jeong/Desktop/dex660-202511
- STUDENT_FILE=/Users/yehan.jeong/Desktop/DEX660-WI25v1-EN-Student-Files

## Anypoint Platform Information
- Mule Account: yehan202511

### Business Group
- Business Group ID: f4d638fd-fc9b-4794-b898-9a02a289e0be
- Client ID: eda99d17552b4388b48b1591aad362ac
- Client Secret: 7DF59c4b13534F82AB84508E1DC035Dd

### Connected App 
- Exchange Contributor ID: 36178f9e1cbb4cceb10af6be312ef9af
- Exchange Contributor Secret: 5c188645417F4aA5b5bd627aB280e920
- CloudHub Deployment ID: 79714db16e854f15883a07bb36cf98c7
- CloudHub Deployment Secret: 446451E13B3c4b39bf660bDb519709b0

### API Instance ID:
- prod: 20609558
- test: 20611526
- dev: 20611518

## Commands
- export PROJECT_HOME=/Users/yehan.jeong/Desktop/dex660-202511
- export STUDENT_FILE=/Users/yehan.jeong/Desktop/DEX660-WI25v1-EN-Student-Files
- curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://localhost:8081/api/v1/tickets/PNR123/checkin
- -M-Danypoint.platform.client_id=eda99d17552b4388b48b1591aad362ac -M-Danypoint.platform.client_secret=7DF59c4b13534F82AB84508E1DC035Dd
- mvn clean verify
- mvn clean deploy
- mvn clean deploy -DmuleDeploy -Dap.client_id=eda99d17552b4388b48b1591aad362ac -Dap.client_secret=7DF59c4b13534F82AB84508E1DC035Dd -Dap.ca.client_id=79714db16e854f15883a07bb36cf98c7 -Dap.ca.client_secret=446451E13B3c4b39bf660bDb519709b0
- curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://check-in-papi-i8dem6.5sc6y6-2.usa-e2.cloudhub.io/api/v1/tickets/PNR123/checkin
- mvn clean deploy -Dencrypt.key=secure12345
- mvn clean deploy -DmuleDeploy -Dap.client_id=eda99d17552b4388b48b1591aad362ac -Dap.client_secret=7DF59c4b13534F82AB84508E1DC035Dd -Dap.ca.client_id=79714db16e854f15883a07bb36cf98c7 -Dap.ca.client_secret=446451E13B3c4b39bf660bDb519709b0 -Dencrypt.key=secure12345 -Ddeployment.env=dev
