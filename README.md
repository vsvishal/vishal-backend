# vishal-backend

```javascript
const app = express();
// app.use() is mostly use when you want to use middleware or do configuration setting
app.use();
```
## Middleware 
- It is a function which runs before any route
- There can be any number of middleware
- When middleware is run it jam the request so need to push using next()

## Express Js
- Express Js is a package behind the scenes that uses node.js Http to create a server.
- We can also create a server directly using node.js HTTP but it will become very difficult and long code to create simple tasks.
- To avoid this we use Express JS
