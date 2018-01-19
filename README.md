# User-Notes-with-Authentication
Requirements

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

5. Then Login then start submitting messages