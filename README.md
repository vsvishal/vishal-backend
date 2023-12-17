# vishal-backend

```javascript
const app = express();
// app.use() is mostly used when you want to use middleware or do configuration setting
app.use();
```
## Middleware 
- It is a function which runs before any route
- There can be any number of middleware
- When middleware is run it jams the request so need to push using next()

## Express Js
- Express Js is a package behind the scenes that uses node.js Http to create a server.
- We can also create a server directly using node.js HTTP but it will become very difficult and long code to create simple tasks.
- To avoid this we use Express JS

## req, res
- req: User data, like I want to know what data the user has sent.
- res: For sending any data from the server, it is sent through res.
- req mai sara data hota hai aane wale user ki, request ki taraf ka, jaise ki uski location, device info, and other things.
- res mai controls hote hai jinke basis pe hum sreve se response bhej pate hai.
- next is just a push so that our req moves to the next things that should be executed.

## Dynamic route
- To make any route dynamic you can use ":" at the place where you want to make it dynamic, and to access their value use "req.params"
- /author/books/issued/:username


## EJS is a like a HTML with computing power, because in normal HTML 1+2 will give 1+2 as output, but in ejs it will compute and give 3.
