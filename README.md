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
- Exchange Contributor ID: 
- Exchange Contributor Secret: 
- CloudHub Deployment ID: 
- CloudHub Deployment Secret: 

### API Instance ID:
- prod: 20609558
- test:
- dev:

## Commands
- export PROJECT_HOME=/Users/yehan.jeong/Desktop/dex660-202511
- export STUDENT_FILE=/Users/yehan.jeong/Desktop/DEX660-WI25v1-EN-Student-Files
- curl -ik -X PUT -H "Content-Type: application/json" -d "{\"lastName\":\"Smith\",\"numBags\":2}" https://localhost:8081/api/v1/tickets/PNR123/checkin
- -M-Danypoint.platform.client_id=eda99d17552b4388b48b1591aad362ac -M-Danypoint.platform.client_secret=7DF59c4b13534F82AB84508E1DC035Dd
-