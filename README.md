# User-Notes-with-Authentication

![Alt text](usernotes1.png?raw=true "Title")

![Alt text](usernotes2.png?raw=true "Title")

## Requirements: AngularJS, Grunt, https-server.

## Deployment Instructions;

1. Clone Project

2. Create FBCreds file with firebase credentials setting the search index to

3. CD into lib folder and run npm install

4. Set Up Firebase with the following rules:
{
  "rules": {
    ".read": "true",
    ".write": "true",
      "notes" : {
        ".indexOn": ["uid"]
      }
    
  }
}
5. Run Https-server with $ hs

6. Open browser with $ http://localhost:8080

7. Register and Login then start submitting messages.