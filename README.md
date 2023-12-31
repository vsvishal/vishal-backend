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


## EJS 
- It is template engine
- It is like HTML with computing power, because in normal HTML 1+2 will give 1+2 as output, but in ejs it will compute and give 3.
- ejs setup steps
  1. ejs install - npm i ejs
  2. configure ejs - app.set("view engine", "ejs");
  3. create one "views" folder & create ejs files in it.
  4. instead of send, do render => render karte waqt make sure app views folder ke aandar wali hi koi file ka naam likhiye, aur render() ma .ejs mention na kare.
 
## Static files (images, stylesheets, javascripts) to setup this follow below steps
- Create a folder public
- Create 3 folders inside it, images, stylesheets, javascript
- Configure the express static in index.js file  


## express generator
- Express generator ek folder bana ke deta hai, jiska matlab aapko khudse folder nhi banana hai, to express gen sare files to is folder ma dal k dega.
- npm i express-generator -g
- express appname --view=ejs  (e.g express vishal --view=ejs]
- cd appname
- npm i
- npx nodemon (to run)

## Database
![image](https://github.com/vsvishal/vishal-backend/assets/39647664/823ae5c8-f27e-4a9e-b493-775deca7987b)
- Ek app ka pura data => db
- Ek app mai variety of data hota hai par poora data hota app ka ki hai, par us data ka sub-category kehlata hai collection
- Collection matalab users ka data, but us me se ak user matlab document.

- - install mongodb
  - install mongoosejs (npm i moongose)
  - require and setup connection
  - make schema
  - create modal and export

