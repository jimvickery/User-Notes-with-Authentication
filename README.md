# User-Notes-with-Authentication

User notes is a CRUD app with authentication built with AngularJS, Javascript, Firebase and Grunt.

## Requirements: AngularJS, Grunt, https-server.

![Alt text](usernotes1.png?raw=true "Title")
<br /><br />

![Alt text](usernotes2.png?raw=true "Title")



## Deployment Instructions;

```
1. Clone Project
```

2. Create FBCreds file with firebase credentials setting the search index to

3. CD into lib folder and in the terminal type:
```
 npm install
 ```

4. Set Up Firebase with the following rules:
```
{
  "rules": {
    ".read": "true",
    ".write": "true",
      "notes" : {
        ".indexOn": ["uid"]
      }
    
  }
}
```
5. Start Https-server in the terminal by typing: 
```  
hs 
```

6. Open browser and type: 
``` 
http://localhost:8080 
```

7. Register and Login then start submitting messages.