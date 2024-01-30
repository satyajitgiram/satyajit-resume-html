### Generate GoogleSheet access "keys.json"

- Create Project in Google Developer Console and enabling Service A/C using google sheet api.

- Go to https://console.cloud.google.com/home/dashboard 

- Create a New Project, Keep Organization as "no organization", Click "Create".

- Once the Project is created Go to Project Dashboard:

- Go to "Explore and Enable API'S under Getting started section", then go to "+ Enable API'S AND SERVICES".
- Search for "Google Sheet Api", Click on "Enable" and after that go to "Credentials" , and under Service account , go to "manage service accounts".
- Provide the "service account name" as per your choice , and make sure to "copy the service account id"
- click on " create and continue", than provide service account access, by choosing "Project" -> "Editor", Click "Done".
- Create A Blank Google sheet & Share the COPIED SERVICE ACCOUNT ID to the google sheet's share with people.
- Go to your service aacount click on "Email" and than in below go to "ADD KEY" choose create new key as json, json file will be downloaded, which is i config.py
- Also get the Spreadsheet_ID from the google-sheet url where you want to save/access the data

``` 
config.py

SERVICE_ACCOUNT_FILE = 'keys.json'
SAMPLE_SPREADSHEET_ID = '1dFcqBGnKJEwl4JCVq_bp-HRINR2hPXKZNy7S7SARZQQ' #GOOGLE SPREADSHEET ID(GoogleSheet URL ID)
```
### Run project
``` 
git clone https://github.com/atulasati/Talmud-Selenium-GoogleSheetAPI.git 
cd Talmud-Selenium-GoogleSheetAPI
pip install -r requirements.txt
python talmud.py
``` 
"# satyajit-resume-html" 
