# New project
Create project 

# API Library
Enable YouTube Data API v3

# Credentials 
Copy and Paste API Key 

# Main
1. Change directory to folder 
2. Install google-apis
```angular2html
pip3 install google-api-python-client
```
3. Import packages
```angular2html
from googleapiclient.discovery import build
```
4. Input details
```angular2html
youtube = build('youtube','v3','AIzaSyDng6iRMnGAy3BQAgL6nUIKfD5HGbHpJns')
```
5. Request
```angular2html
request = youtube.channels().list(
part = 'statistics'
forUsername = 'joeychua'
)
```
6. Response
```
response = request.execute()
print(response)
```

