tika-jar
========

Just a convenient way to distribute Apache Tika jar for usage in your Node.js project

Include it in your beautiful `package.json`
```json
"dependencies": {
  "tika-jar": "https://github.com/beyondcompute/tika-jar/archive/1.6.0.tar.gz"
}
```

Then use it from your code like this:
```javascript
var exec = require('child_process').exec;

exec('java -Djava.awt.headless=true -jar ../node_modules/tika-jar/tika-app-1.6.jar --text < ' + filename, function(err, stdout, stderr) {
  // stdout is the contents of your parsed document
});
```
