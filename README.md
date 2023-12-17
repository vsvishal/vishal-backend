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
