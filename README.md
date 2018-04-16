# README

#### Details

- rails (5.1.6)
- sqlite3 (1.3.13)

#### Snippets
**AJAX Request Snippet**

```
var blocmetrics = {};
blocmetrics.report = function(eventName){
  var event = {event: { name: eventName }};
  var request = new XMLHttpRequest();

  request.open("POST", "http://localhost:3000/api/events", true);
  request.setRequestHeader('Content-Type', 'application/json');
  request.send(JSON.stringify(event));
};
```
