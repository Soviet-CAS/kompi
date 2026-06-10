# Node.js Complete Tutorial - From Beginner to Advanced

**មេរៀន Node.js ពីចាប់ផ្តើម ដល់កម្រិតខ្ពស់**
Learn Node.js from Middlewares from scratch to building production-ready applications

រៀន Node.js ពីដំបូង រហូតដល់អភិវឌ្ឍកម្មវិធីពិតប្រាកដ

## Table of Contents

- [1. Beginner Level](#1.-beginner-level)
- [2. Intermediate Level](#2.-intermediate-level)
- [3. Database & Storage](#3.-database-storage)
- [4. Authentication & Security](#4.-authentication-security)
- [5. Advanced Node.js](#5.-advanced-node.js)
- [Additional Resources](#additional-resources)

## 1. Beginner Level

**កម្រិតចាប់ផ្តើម**
Fundamental concepts and setup for Node.js beginners

គោលគំនិតមូលដ្ឋាន និងការដំឡើងសម្រាប់អ្នកចាប់ផ្តើមរៀន Node.js

### 1. Introduction to Node.js

### ១. ការណែនាំអំពី Node.js
Node.js is a JavaScript runtime built on Chrome's V8 engine for server-side development.

Node.js គឺជាបរិយាកាស JavaScript runtime ដែលបង្កើតឡើងលើ Chrome's V8 engine សម្រាប់ការអភិវឌ្ឍនៅផ្នែក server។

#### Example

```javascript
// First Node.js program
console.log('Hello, Node.js!');
console.log('Node.js version:', process.version);
```

#### Explanation
កូដនេះបង្ហាញសារសាមញ្ញ 'Hello, Node.js!' និងបង្ហាញកំណែ Node.js ដែលកំពុងប្រើ។ `process.version` ផ្តល់ព័ត៌មានអំពីកំណែ Node.js។

#### Output

```text
Hello, Node.js!
Node.js version: v18.17.0
```

#### Summary / សរុប
ជំពូកនេះណែនាំ Node.js ដែលជាបរិយាកាសសម្រាប់ដំណើរការ JavaScript នៅផ្នែក server។ វាពន្យល់ពីគោលគំនិតមូលដ្ឋាន និងបង្ហាញកម្មវិធី Node.js ដំបូង។

### 2. Installing Node.js & npm

### ២. ការដំឡើង Node.js និង npm
Guide to installing Node.js and npm on various operating systems.

ការណែនាំអំពីការដំឡើង Node.js និង npm នៅលើប្រព័ន្ធប្រតិបត្តិការផ្សេងៗ។

#### Example

```bash
# Ubuntu/Debian
sudo apt update
sudo apt install nodejs npm

# Verify installation
node --version
npm --version
```

#### Explanation
កូដនេះបង្ហាញពីរបៀបដំឡើង Node.js និង npm នៅលើប្រព័ន្ធ Ubuntu/Debian ដោយប្រើ `apt`។ បន្ទាប់មក ពិនិត្យកំណែដែលបានដំឡើងដោយប្រើ `node --version` និង `npm --version`។

#### Output

```text
v18.17.0
9.6.7
```

#### Summary / សរុប
ជំពូកនេះណែនាំពីរបៀបដំឡើង Node.js និង npm ដែលជាកម្មវិធីគ្រប់គ្រងកញ្ចប់ នៅលើប្រព័ន្ធប្រតិបត្តិការផ្សេងៗ។

### 3. Running Your First Node.js Program

### ៣. ដំណើរការកម្មវិធី Node.js ដំបូង
Create and run a simple Node.js program.

បង្កើត និងដំណើរការកម្មវិធី Node.js សាមញ្ញ។

#### Example

```javascript
// app.js
console.log('Hello, Node.js World!');
console.log('Current time:', new Date().toLocaleString());
```

#### Explanation
កូដនេះបង្កើតឯកសារ `app.js` ដែលបង្ហាញសារ 'Hello, Node.js World!' និងបង្ហាញពេលវេលាបច្ចុប្បន្នដោយប្រើ `new Date().toLocaleString()`។ ដំណើរការដោយប្រើ `node app.js`។

#### Output

```text
Hello, Node.js World!
Current time: 8/18/2025, 4:19:00 PM
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីរបៀបបង្កើត និងដំណើរការកម្មវិធី Node.js ដំបូង ដោយប្រើសារសាមញ្ញ និងការបង្ហាញពេលវេលា។

### 4. Understanding Modules & require()

### ៤. ការយល់ដឹងអំពីម៉ូឌុល និង require()
Learn about Node.js modules and the require() function.

ស្វែងយល់អំពីម៉ូឌុល Node.js និងមុខងារ require()។

#### Example

```javascript
// math.js
exports.add = (a, b) => a + b;

// app.js
const math = require('./math');
console.log(math.add(2, 3));
```

#### Explanation
កូដនេះបង្កើតម៉ូឌុល `math.js` ដែលមានមុខងារបូកលេខ។ នៅក្នុង `app.js` យើងនាំចូលម៉ូឌុលនេះដោយប្រើ `require()` និងហៅមុខងារ `add` ដើម្បីបូក 2 និង 3។

#### Output

```text
5
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីម៉ូឌុល និងការប្រើ `require()` ដើម្បីនាំចូលមុខងារពីឯកសារមួយទៅឯកសារមួយទៀត។

### 5. Node.js REPL (Read-Eval-Print-Loop)

### ៥. Node.js REPL (អាន-វាយតម្លៃ-បោះពុម្ព-រង្វិលជុំ)
Use the Node.js REPL for interactive JavaScript coding.

ប្រើ Node.js REPL សម្រាប់ការសរសេរកូដ JavaScript ដោយអន្តរកម្ម។

#### Example

```bash
# Start REPL
node
> console.log('Hello from REPL!');
> .exit
```

#### Explanation
កូដនេះបង្ហាញពីរបៀបចាប់ផ្តើម REPL ដោយវាយ `node` នៅក្នុង terminal។ បន្ទាប់មក យើងសរសេរកូដ `console.log` ដើម្បីបង្ហាញសារ និងប្រើ `.exit` ដើម្បីចាកចេញ។

#### Output

```text
Hello from REPL!
```

#### Summary / សរុប
ជំពូកនេះណែនាំពី REPL ដែលជាឧបករណ៍អន្តរកម្មសម្រាប់សាកល្បងកូដ JavaScript នៅក្នុង Node.js។

### 6. File System (fs) Module

### ៦. ម៉ូឌុលប្រព័ន្ធឯកសារ (fs)
Work with the file system using the fs module.

ធ្វើការជាមួយប្រព័ន្ធឯកសារដោយប្រើម៉ូឌុល fs។

#### Example

```javascript
const fs = require('fs');
fs.writeFileSync('example.txt', 'Hello, Node.js!');
const data = fs.readFileSync('example.txt', 'utf8');
console.log(data);
```

#### Explanation
កូដនេះប្រើម៉ូឌុល `fs` ដើម្បីសរសេរសារ 'Hello, Node.js!' ទៅក្នុងឯកសារ `example.txt` ដោយប្រើ `writeFileSync`។ បន្ទាប់មក អានឯកសារដោយប្រើ `readFileSync` និងបង្ហាញខ្លឹមសារ។

#### Output

```text
Hello, Node.js!
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីរបៀបប្រើម៉ូឌុល `fs` ដើម្បីអាន និងសរសេរឯកសារនៅក្នុង Node.js។

### 7. Path Module

### ៧. ម៉ូឌុល Path
Handle file paths using the path module.

គ្រប់គ្រងផ្លូវឯកសារដោយប្រើម៉ូឌុល path។

#### Example

```javascript
const path = require('path');
const fullPath = path.join('/users', 'john', 'file.txt');
console.log(fullPath);
```

#### Explanation
កូដនេះប្រើម៉ូឌុល `path` ដើម្បីភ្ជាប់ផ្លូវឯកសារដោយប្រើ `path.join`។ វាបញ្ចូលផ្នែកផ្លូវ `/users`, `john`, និង `file.txt` ទៅជាផ្លូវពេញលេញ។

#### Output

```text
/users/john/file.txt
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការប្រើម៉ូឌុល `path` ដើម្បីគ្រប់គ្រងផ្លូវឯកសារប្រកបដោយប្រសិទ្ធភាព។

### 8. Events & EventEmitter

### ៨. ព្រឹត្តិការណ៍ និង EventEmitter
Handle events using the EventEmitter class.

គ្រប់គ្រងព្រឹត្តិការណ៍ដោយប្រើថ្នាក់ EventEmitter។

#### Example

```javascript
const EventEmitter = require('events');
const emitter = new EventEmitter();
emitter.on('greet', (name) => console.log(`Hello, ${name}!`));
emitter.emit('greet', 'John');
```

#### Explanation
កូដនេះប្រើ `EventEmitter` ដើម្បីបង្កើតព្រឹត្តិការណ៍ `greet`។ នៅពេល `emit` ត្រូវបានហៅជាមួយឈ្មោះ 'John' វាបង្ហាញសារ 'Hello, John!'។

#### Output

```text
Hello, John!
```

#### Summary / សរុប
ជំពូកនេះណែនាំពី `EventEmitter` សម្រាប់គ្រប់គ្រងព្រឹត្តិការណ៍នៅក្នុង Node.js។

### 9. Understanding Callbacks & Async Programming

### ៩. ការយល់ដឹងអំពី Callbacks និងការសរសេរកម្មវិធីអសមកាល
Learn about callbacks and asynchronous programming in Node.js.

ស្វែងយល់អំពី callbacks និងការសរសេរកម្មវិធីអសមកាលនៅក្នុង Node.js។

#### Example

```javascript
const fs = require('fs');
fs.readFile('example.txt', 'utf8', (err, data) => {
  if (err) console.error(err);
  console.log(data);
});
```

#### Explanation
កូដនេះប្រើ `fs.readFile` ដើម្បីអានឯកសារដោយអសមកាល។ Callback មុខងារនឹងត្រូវបានហៅនៅពេលអានរួច ដោយបង្ហាញខ្លឹមសារឯកសារ ឬកំហុសប្រសិនបើមាន។

#### Output

```text
Hello, Node.js!
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពី callbacks និងការសរសេរកម្មវិធីអសមកាល ដែលជាគោលគំនិតសំខាន់នៅក្នុង Node.js។

### 10. Using npm & package.json

### ១០. ការប្រើ npm និង package.json
Manage dependencies using npm and package.json.

គ្រប់គ្រង dependencies ដោយប្រើ npm និង package.json។

#### Example

```bash
# Initialize project
npm init -y
# Install express
npm install express
# package.json
{
  "name": "my-app",
  "version": "1.0.0",
  "dependencies": {
    "express": "^4.18.2"
  }
}
```

#### Explanation
កូដនេះបង្ហាញពីរបៀបចាប់ផ្តើមគម្រោងជាមួយ `npm init -y` និងដំឡើង `express`។ ឯកសារ `package.json` កត់ត្រាព័ត៌មានគម្រោង និង dependencies។

#### Output

```javascript
Project initialized with express installed.
```

#### Summary / សរុប
ជំពូកនេះណែនាំពី npm និង `package.json` សម្រាប់គ្រប់គ្រងកញ្ចប់ និងការកំណត់គម្រោង។

## 2. Intermediate Level

**កម្រិតមធ្យម**
Building web applications and APIs with Node.js.

ការអភិវឌ្ឍកម្មវិធីបណ្តាញ និង API ជាមួយ Node.js។

### 11. HTTP Module – Creating a Web Server

### ១១. ម៉ូឌុល HTTP – បង្កើត Web Server
Create a web server using the built-in HTTP module.

បង្កើត web server ដោយប្រើម៉ូឌុល HTTP ដែលមានស្រាប់។

#### Example

```javascript
const http = require('http');
const server = http.createServer((req, res) => {
  res.writeHead(200, { 'Content-Type': 'text/plain' });
  res.end('Hello, World!');
});
server.listen(3000, () => console.log('Server running on port 3000'));
```

#### Explanation
កូដនេះប្រើម៉ូឌុល `http` ដើម្បីបង្កើត server ដែលឆ្លើយតបជាមួយសារ 'Hello, World!' នៅពេលចូលទៅកាន់ port 3000។ `createServer` បង្កើត server និង `listen` ចាប់ផ្តើមវា។

#### Output

```text
Server running on port 3000
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបង្កើត web server សាមញ្ញដោយប្រើម៉ូឌុល `http`។

### 12. Express.js Framework Basics

### ១២. មូលដ្ឋាន Express.js Framework
Introduction to the Express.js web framework.

ការណែនាំអំពី framework បណ្តាញ Express.js។

#### Example

```javascript
const express = require('express');
const app = express();
app.get('/', (req, res) => res.send('Hello from Express!'));
app.listen(3000, () => console.log('Server running'));
```

#### Explanation
កូដនេះប្រើ `express` ដើម្បីបង្កើត server។ នៅពេលចូលទៅកាន់ root URL (`/`), វាឆ្លើយតបជាមួយសារ 'Hello from Express!'។ `app.listen` ចាប់ផ្តើម server នៅ port 3000។

#### Output

```text
Server running
```

#### Summary / សរុប
ជំពូកនេះណែនាំពី Express.js និងរបៀបបង្កើត server បណ្តាញសាមញ្ញ។

### 13. Middleware in Express

### ១៣. Middleware ក្នុង Express
Use middleware to handle requests in Express.

ប្រើ middleware ដើម្បីគ្រប់គ្រងសំណើនៅក្នុង Express។

#### Example

```javascript
const express = require('express');
const app = express();
const logger = (req, res, next) => {
  console.log(`${req.method} ${req.url}`);
  next();
};
app.use(logger);
app.get('/', (req, res) => res.send('Hello!'));
app.listen(3000);
```

#### Explanation
កូដនេះបង្កើត middleware `logger` ដែលកត់ត្រាវិធីសាស្ត្រ HTTP និង URL នៃសំណើ។ `app.use` អនុវត្ត middleware ទៅគ្រប់សំណើ និង `next()` អនុញ្ញាតឱ្យបន្តទៅ route បន្ទាប់។

#### Output

```text
GET /
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពី middleware នៅក្នុង Express ដែលជួយគ្រប់គ្រងសំណើមុនពេលឆ្លើយតប។

### 14. Routing in Express

### ១៤. Routing ក្នុង Express
Define routes to handle different endpoints in Express.

កំណត់ routes ដើម្បីគ្រប់គ្រង endpoints ផ្សេងៗនៅក្នុង Express។

#### Example

```javascript
const express = require('express');
const app = express();
app.get('/users/:id', (req, res) => res.send(`User ${req.params.id}`));
app.listen(3000);
```

#### Explanation
កូដនេះកំណត់ route `/users/:id` ដែលទទួលប៉ារ៉ាម៉ែត្រ `id` ពី URL។ នៅពេលចូលទៅ `/users/1`, វាឆ្លើយតបជាមួយ 'User 1'។

#### Output

```text
User 1
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការកំណត់ routes នៅក្នុង Express ដើម្បីឆ្លើយតបទៅនឹងសំណើ URL ផ្សេងៗ។

### 15. Handling Forms & JSON Data

### ១៥. ការគ្រប់គ្រងទម្រង់ និងទិន្នន័យ JSON
Process form submissions and JSON data in Express.

ដំណើរការទម្រង់បញ្ជូន និងទិន្នន័យ JSON នៅក្នុង Express។

#### Example

```javascript
const express = require('express');
const app = express();
app.use(express.json());
app.post('/api/data', (req, res) => res.json(req.body));
app.listen(3000);
```

#### Explanation
កូដនេះប្រើ `express.json()` ដើម្បីបកប្រែទិន្នន័យ JSON ពីសំណើ POST។ Route `/api/data` ឆ្លើយតបជាមួយទិន្នន័យដែលបានបញ្ជូន។

#### Output

```json
{ "name": "John" }
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការគ្រប់គ្រងទម្រង់ និងទិន្នន័យ JSON នៅក្នុង Express។

### 16. REST API with Express

### ១៦. REST API ជាមួយ Express
Build a RESTful API using Express.

អភិវឌ្ឍ RESTful API ដោយប្រើ Express។

#### Example

```javascript
const express = require('express');
const app = express();
app.use(express.json());
let users = [];
app.post('/api/users', (req, res) => {
  users.push(req.body);
  res.status(201).json(req.body);
});
app.get('/api/users', (req, res) => res.json(users));
app.listen(3000);
```

#### Explanation
កូដនេះបង្កើត REST API ជាមួយ routes សម្រាប់បង្កើត (POST) និងទទួល (GET) ទិន្នន័យអ្នកប្រើ។ `users` ជាអារេដែលរក្សាទុកទិន្នន័យ។

#### Output

```json
[{ "name": "John" }]
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបង្កើត REST API ដោយប្រើ Express សម្រាប់គ្រប់គ្រងទិន្នន័យ។

### 17. Working with Query Strings & URL Parameters

### ១៧. ការធ្វើការជាមួយ Query Strings និងប៉ារ៉ាម៉ែត្រ URL
Handle query strings and URL parameters in Express.

គ្រប់គ្រង query strings និងប៉ារ៉ាម៉ែត្រ URL នៅក្នុង Express។

#### Example

```javascript
const express = require('express');
const app = express();
app.get('/search', (req, res) => res.json(req.query));
app.listen(3000);
```

#### Explanation
កូដនេះបង្កើត route `/search` ដែលទទួល query strings (ឧ. `/search?q=nodejs`) និងឆ្លើយតបជាមួយទិន្នន័យ query។

#### Output

```json
{ "q": "nodejs" }
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការគ្រប់គ្រង query strings និងប៉ារ៉ាម៉ែត្រ URL នៅក្នុង Express។

### 18. Template Engines (EJS, Handlebars, Pug)

### ១៨. Template Engines (EJS, Handlebars, Pug)
Use template engines to render dynamic HTML.

ប្រើ template engines ដើម្បីបង្កើត HTML ដែលមានភាពថាមវន្ត។

#### Example

```javascript
const express = require('express');
const app = express();
app.set('view engine', 'ejs');
app.get('/', (req, res) => res.render('index', { name: 'John' }));
app.listen(3000);
```

#### Explanation
កូដនេះប្រើ EJS ជា template engine។ Route `/` បង្ហាញ template `index.ejs` ជាមួយទិន្នន័យ `name`។

#### Output

```text
Rendered HTML with name 'John'
```

#### Summary / សរុប
ជំពូកនេះណែនាំពី template engines ដូចជា EJS សម្រាប់បង្កើត HTML ថាមវន្ត។

### 19. Error Handling in Node.js

### ១៩. ការគ្រប់គ្រងកំហុសនៅក្នុង Node.js
Handle errors gracefully in Node.js applications.

គ្រប់គ្រងកំហុសប្រកបដោយប្រសិទ្ធភាពនៅក្នុងកម្មវិធី Node.js។

#### Example

```javascript
const express = require('express');
const app = express();
app.get('/', (req, res, next) => {
  try {
    throw new Error('Something went wrong');
  } catch (err) {
    next(err);
  }
});
app.use((err, req, res, next) => res.status(500).json({ error: err.message }));
app.listen(3000);
```

#### Explanation
កូដនេះបង្ហាញការគ្រប់គ្រងកំហុសនៅក្នុង Express។ ប្រសិនបើមានកំហុស វាត្រូវបានបញ្ជូនទៅ middleware ដែលឆ្លើយតបជាមួយសារ។

#### Output

```json
{ "error": "Something went wrong" }
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការគ្រប់គ្រងកំហុសនៅក្នុង Node.js ដើម្បីធានាបទពិសោធន៍អ្នកប្រើប្រសើរឡើង។

### 20. Debugging & Logging

### ២០. ការបំបាត់កំហុស និងការកត់ត្រា
Debug and log issues in Node.js applications.

បំបាត់កំហុស និងកត់ត្រាបញ្ហានៅក្នុងកម្មវិធី Node.js។

#### Example

```javascript
const winston = require('winston');
const logger = winston.createLogger({
  transports: [new winston.transports.File({ filename: 'app.log' })]
});
logger.info('Application started');
console.log('Debugging...');
```

#### Explanation
កូដនេះប្រើ `winston` ដើម្បីកត់ត្រាសារទៅក្នុងឯកសារ `app.log`។ `console.log` ប្រើសម្រាប់បំបាត់កំហុសសាមញ្ញ។

#### Output

```javascript
Application started (logged to app.log)
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការបំបាត់កំហុស និងការកត់ត្រាដើម្បីតាមដានបញ្ហានៅក្នុងកម្មវិធី។

## 3. Database & Storage

**មូលដ្ឋានទិន្នន័យ និងការផ្ទុក**
Integrate databases and storage solutions with Node.js.

ភ្ជាប់មូលដ្ឋានទិន្នន័យ និងដំណោះស្រាយការផ្ទុកជាមួយ Node.js។

### 21. Introduction to Databases in Node.js

### ២១. ការណែនាំអំពីមូលដ្ឋានទិន្នន័យនៅក្នុង Node.js
Overview of database integration in Node.js.

ទិដ្ឋភាពទូទៅនៃការភ្ជាប់មូលដ្ឋានទិន្នន័យនៅក្នុង Node.js។

#### Example

```javascript
// Example placeholder for database connection
const db = require('some-db-driver');
// Connect to database
db.connect('connection-string');
```

#### Explanation
កូដនេះជាឧទាហរណ៍សម្រាប់ភ្ជាប់ទៅមូលដ្ឋានទិន្នន័យដោយប្រើ driver ជាក់លាក់។

#### Output

```text
Database connected
```

#### Summary / សរុប
ជំពូកនេះផ្តល់ទិដ្ឋភាពទូទៅអំពីការភ្ជាប់មូលដ្ឋានទិន្នន័យជាមួយ Node.js។

### 22. MongoDB with Mongoose

### ២២. MongoDB ជាមួយ Mongoose
Use MongoDB with Mongoose for NoSQL database operations.

ប្រើ MongoDB ជាមួយ Mongoose សម្រាប់ប្រតិបត្តិការមូលដ្ឋានទិន្នន័យ NoSQL។

#### Example

```javascript
const mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/myapp');
const User = mongoose.model('User', new mongoose.Schema({ name: String }));
const user = new User({ name: 'John' });
user.save().then(() => console.log('User saved'));
```

#### Explanation
កូដនេះភ្ជាប់ទៅ MongoDB ដោយប្រើ `mongoose`។ បង្កើត model `User` និងរក្សាទុកអ្នកប្រើថ្មីជាមួយឈ្មោះ 'John'។

#### Output

```text
User saved
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ MongoDB និង Mongoose សម្រាប់គ្រប់គ្រងទិន្នន័យ NoSQL។

### 23. MySQL with Node.js

### ២៣. MySQL ជាមួយ Node.js
Connect to MySQL databases using Node.js.

ភ្ជាប់ទៅមូលដ្ឋានទិន្នន័យ MySQL ដោយប្រើ Node.js។

#### Example

```javascript
const mysql = require('mysql2');
const connection = mysql.createConnection({ host: 'localhost', user: 'root', database: 'myapp' });
connection.query('SELECT * FROM users', (err, results) => console.log(results));
```

#### Explanation
កូដនេះភ្ជាប់ទៅ MySQL និងអនុវត្ត query ដើម្បីទទួលទិន្នន័យអ្នកប្រើ។ `mysql2` ជា driver សម្រាប់ MySQL។

#### Output

```json
[{ id: 1, name: 'John' }]
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការភ្ជាប់ និងធ្វើការជាមួយ MySQL នៅក្នុង Node.js។

### 24. PostgreSQL with Node.js

### ២៤. PostgreSQL ជាមួយ Node.js
Integrate PostgreSQL with Node.js applications.

ភ្ជាប់ PostgreSQL ជាមួយកម្មវិធី Node.js។

#### Example

```javascript
const { Pool } = require('pg');
const pool = new Pool({ user: 'root', host: 'localhost', database: 'myapp' });
pool.query('SELECT * FROM users', (err, res) => console.log(res.rows));
```

#### Explanation
កូដនេះប្រើ `pg` ដើម្បីភ្ជាប់ទៅ PostgreSQL និងទាញយកទិន្នន័យអ្នកប្រើ។ `Pool` គ្រប់គ្រងការភ្ជាប់។

#### Output

```json
[{ id: 1, name: 'John' }]
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការភ្ជាប់ PostgreSQL និងការធ្វើ query នៅក្នុង Node.js។

### 25. Redis Caching with Node.js

### ២៥. Redis Caching ជាមួយ Node.js
Use Redis for caching in Node.js applications.

ប្រើ Redis សម្រាប់ caching នៅក្នុងកម្មវិធី Node.js។

#### Example

```javascript
const redis = require('redis');
const client = redis.createClient();
client.set('key', 'value');
client.get('key', (err, reply) => console.log(reply));
```

#### Explanation
កូដនេះភ្ជាប់ទៅ Redis និងរក្សាទុកគន្លឹះ-តម្លៃ ('key', 'value')។ `client.get` ទាញយកតម្លៃ។

#### Output

```text
value
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការប្រើ Redis សម្រាប់ caching ដើម្បីបង្កើនល្បឿនកម្មវិធី។

### 26. File Upload & Storage (Multer, Cloud Storage)

### ២៦. ការបញ្ចូនឯកសារ និងការផ្ទុក (Multer, Cloud Storage)
Handle file uploads and cloud storage in Node.js.

គ្រប់គ្រងការបញ្ចូនឯកសារ និងការផ្ទុកនៅលើ cloud ក្នុង Node.js។

#### Example

```javascript
const express = require('express');
const multer = require('multer');
const upload = multer({ dest: 'uploads/' });
const app = express();
app.post('/upload', upload.single('file'), (req, res) => res.send('File uploaded'));
app.listen(3000);
```

#### Explanation
កូដនេះប្រើ `multer` ដើម្បីគ្រប់គ្រងការបញ្ចូនឯកសារ។ Route `/upload` ទទួលឯកសារតែមួយ និងរក្សាទុកនៅថត `uploads/`។

#### Output

```text
File uploaded
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបញ្ចូនឯកសារដោយប្រើ `multer` និងការផ្ទុកនៅលើ cloud។

## 4. Authentication & Security

**ការផ្ទៀងផ្ទាត់ និងសុវត្ថិភាព**
Implement secure authentication and authorization.

អនុវត្តការផ្ទៀងផ្ទាត់ និងការអនុញ្ញាតប្រកបដោយសុវត្ថិភាព។

### 27. Authentication Basics

### ២៧. មូលដ្ឋាននៃការផ្ទៀងផ្ទាត់
Understand authentication concepts in Node.js.

យល់ដឹងអំពីគោលគំនិតនៃការផ្ទៀងផ្ទាត់នៅក្នុង Node.js។

#### Example

```javascript
const express = require('express');
const app = express();
app.use(express.json());
app.post('/login', (req, res) => {
  const { username, password } = req.body;
  if (username === 'admin' && password === 'pass') res.json({ token: 'abc123' });
  else res.status(401).json({ error: 'Invalid credentials' });
});
app.listen(3000);
```

#### Explanation
កូដនេះបង្កើត endpoint `/login` សម្រាប់ផ្ទៀងផ្ទាត់អ្នកប្រើ។ ប្រសិនបើ username និង password ត្រឹមត្រូវ វាផ្តល់ token។

#### Output

```json
{ "token": "abc123" }
```

#### Summary / សរុប
ជំពូកនេះណែនាំពីគោលគំនិតនៃការផ្ទៀងផ្ទាត់អ្នកប្រើនៅក្នុង Node.js។

### 28. JSON Web Tokens (JWT)

### ២៨. JSON Web Tokens (JWT)
Implement JWT for secure authentication.

អនុវត្ត JWT សម្រាប់ការផ្ទៀងផ្ទាត់ប្រកបដោយសុវត្ថិភាព។

#### Example

```javascript
const jwt = require('jsonwebtoken');
const token = jwt.sign({ userId: 1 }, 'secret', { expiresIn: '1h' });
console.log(token);
```

#### Explanation
កូដនេះប្រើ `jsonwebtoken` ដើម្បីបង្កើត JWT token ដែលមាន `userId` និងផុតកំណត់ក្នុង 1 ម៉ោង។

#### Output

```text
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ JWT សម្រាប់ការផ្ទៀងផ្ទាត់ប្រកបដោយសុវត្ថិភាព។

### 29. Sessions & Cookies

### ២៩. Sessions និង Cookies
Manage user sessions and cookies in Node.js.

គ្រប់គ្រង sessions និង cookies របស់អ្នកប្រើនៅក្នុង Node.js។

#### Example

```javascript
const express = require('express');
const cookieParser = require('cookie-parser');
const app = express();
app.use(cookieParser());
app.get('/', (req, res) => {
  res.cookie('name', 'John');
  res.send('Cookie set');
});
app.listen(3000);
```

#### Explanation
កូដនេះប្រើ `cookie-parser` ដើម្បីកំណត់ cookie `name` ជាមួយតម្លៃ 'John'។

#### Output

```text
Cookie set
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការគ្រប់គ្រង sessions និង cookies នៅក្នុង Node.js។

### 30. Password Hashing (bcrypt, crypto)

### ៣០. ការធ្វើ Hash លើលេខសម្ងាត់ (bcrypt, crypto)
Securely hash passwords using bcrypt or crypto.

ធ្វើ hash លើលេខសម្ងាត់ប្រកបដោយសុវត្ថិភាពដោយប្រើ bcrypt ឬ crypto។

#### Example

```javascript
const bcrypt = require('bcryptjs');
bcrypt.hash('password', 10, (err, hash) => console.log(hash));
```

#### Explanation
កូដនេះប្រើ `bcrypt` ដើម្បីធ្វើ hash លើលេខសម្ងាត់ 'password' ជាមួយ salt rounds 10។

#### Output

```text
$2a$10$...
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការធ្វើ hash លើលេខសម្ងាត់ដើម្បីសុវត្ថិភាព។

### 31. Securing APIs (Helmet, Rate Limiting, CORS)

### ៣១. ការការពារ APIs (Helmet, Rate Limiting, CORS)
Secure APIs with Helmet, rate limiting, and CORS.

ការពារ APIs ដោយប្រើ Helmet, rate limiting, និង CORS។

#### Example

```javascript
const express = require('express');
const helmet = require('helmet');
const app = express();
app.use(helmet());
app.get('/', (req, res) => res.send('Secure API'));
app.listen(3000);
```

#### Explanation
កូដនេះប្រើ `helmet` ដើម្បីបន្ថែម headers សុវត្ថិភាពទៅ API។

#### Output

```text
Secure API
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការការពារ APIs ដោយប្រើឧបករណ៍ដូចជា Helmet និង CORS។

## 5. Advanced Node.js

**Node.js កម្រិតខ្ពស់**
Advanced concepts for building scalable Node.js applications.

គោលគំនិតកម្រិតខ្ពស់សម្រាប់អភិវឌ្ឍកម្មវិធី Node.js ដែលអាចពង្រីកបាន។

### 32. Streams & Buffers

### ៣២. Streams និង Buffers
Handle large data efficiently with streams and buffers.

គ្រប់គ្រងទិន្នន័យធំប្រកបដោយប្រសិទ្ធភាពជាមួយ streams និង buffers។

#### Example

```javascript
const fs = require('fs');
const readStream = fs.createReadStream('large.txt');
readStream.on('data', (chunk) => console.log(chunk.length));
```

#### Explanation
កូដនេះប្រើ `createReadStream` ដើម្បីអានឯកសារធំជាផ្នែកៗ (chunks) និងបង្ហាញទំហំនៃ chunk នីមួយៗ។

#### Output

```text
65536
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពី streams និង buffers សម្រាប់គ្រប់គ្រងទិន្នន័យធំ។

### 33. Child Processes

### ៣៣. Child Processes
Run external processes using child_process module.

ដំណើរការដំណើរការខាងក្រៅដោយប្រើម៉ូឌុល child_process។

#### Example

```javascript
const { exec } = require('child_process');
exec('ls', (err, stdout) => console.log(stdout));
```

#### Explanation
កូដនេះប្រើ `exec` ដើម្បីដំណើរការពាក្យបញ្ជា `ls` និងបង្ហាញឈ្មោះឯកសារនៅក្នុងថត។

#### Output

```text
file1.txt
file2.txt
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ `child_process` ដើម្បីដំណើរការពាក្យបញ្ជាខាងក្រៅ។

### 34. Worker Threads & Clustering

### ៣៤. Worker Threads និង Clustering
Scale applications using worker threads and clustering.

ពង្រីកកម្មវិធីដោយប្រើ worker threads និង clustering។

#### Example

```javascript
const cluster = require('cluster');
if (cluster.isMaster) {
  cluster.fork();
} else {
  console.log('Worker running');
}
```

#### Explanation
កូដនេះប្រើ `cluster` ដើម្បីបង្កើត worker process។ ប្រសិនបើជា master process វាបង្កើត worker ថ្មី។

#### Output

```text
Worker running
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពី worker threads និង clustering សម្រាប់ការពង្រីកកម្មវិធី។

### 35. WebSockets & Real-Time Communication (Socket.io)

### ៣៥. WebSockets និងការទំនាក់ទំនងតាមពេលជាក់ស្តែង (Socket.io)
Implement real-time communication with Socket.io.

អនុវត្តការទំនាក់ទំនងតាមពេលជាក់ស្តែងជាមួយ Socket.io។

#### Example

```javascript
const io = require('socket.io')(3000);
io.on('connection', (socket) => socket.emit('message', 'Hello!'));
```

#### Explanation
កូដនេះបង្កើត WebSocket server ជាមួយ `socket.io` នៅ port 3000 និងផ្ញើសារ 'Hello!' ទៅ client ដែលភ្ជាប់។

#### Output

```text
Hello!
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ Socket.io សម្រាប់ការទំនាក់ទំនងតាមពេលជាក់ស្តែង។

### 36. Event Loop & Async Patterns

### ៣៦. Event Loop និង Async Patterns
Understand the Node.js event loop and async patterns.

យល់ដឹងអំពី event loop និង async patterns នៅក្នុង Node.js។

#### Example

```javascript
setImmediate(() => console.log('Immediate'));
setTimeout(() => console.log('Timeout'), 0);
```

#### Explanation
កូដនេះបង្ហាញពី event loop។ `setImmediate` និង `setTimeout` ដំណើរការដោយអសមកាល ដោយ `setImmediate` មានអាទិភាពខ្ពស់ជាង។

#### Output

```text
Immediate
Timeout
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពី event loop និងរបៀបគ្រប់គ្រងការងារអសមកាល។

### 37. Performance Optimization (caching, scaling)

### ៣៧. ការបង្កើនប្រសិទ្ធភាព (caching, scaling)
Optimize Node.js applications for performance.

បង្កើនប្រសិទ្ធភាពកម្មវិធី Node.js សម្រាប់ការអនុវត្ត។

#### Example

```javascript
const cache = new Map();
function getData(key) {
  if (cache.has(key)) return cache.get(key);
  const data = 'Expensive operation';
  cache.set(key, data);
  return data;
}
console.log(getData('key'));
```

#### Explanation
កូដនេះប្រើ `Map` សម្រាប់ caching ដើម្បីជៀសវាងការគណនាដែលមានតម្លៃថ្លៃ។

#### Output

```text
Expensive operation
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបង្កើនប្រសិទ្ធភាពដោយប្រើ caching និង scaling។

### 38. Testing (Mocha, Jest, Supertest)

### ៣៨. ការធ្វើតេស្ត (Mocha, Jest, Supertest)
Test Node.js applications using Mocha, Jest, and Supertest.

ធ្វើតេស្តកម្មវិធី Node.js ដោយប្រើ Mocha, Jest, និង Supertest។

#### Example

```javascript
const { expect } = require('chai');
describe('Math', () => {
  it('should add numbers', () => expect(1 + 1).to.equal(2));
});
```

#### Explanation
កូដនេះប្រើ `chai` និង Mocha ដើម្បីសាកល្បងថាតើ 1 + 1 ស្មើ 2។

#### Output

```text
Test passed
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការធ្វើតេស្តកម្មវិធីដោយប្រើ Mocha, Jest, និង Supertest។

### 39. Debugging with Node Inspector

### ៣៩. ការបំបាត់កំហុសជាមួយ Node Inspector
Debug Node.js applications using Node Inspector.

បំបាត់កំហុសកម្មវិធី Node.js ដោយប្រើ Node Inspector។

#### Example

```bash
node --inspect app.js
// In browser: chrome://inspect
```

#### Explanation
កូដនេះចាប់ផ្តើម `app.js` ជាមួយ `--inspect` ដើម្បីបើក Node Inspector សម្រាប់បំបាត់កំហុសនៅក្នុង Chrome។

#### Output

```text
Debugger attached
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបំបាត់កំហុសជាមួយ Node Inspector នៅក្នុង browser។

### 40. Environment Variables & dotenv

### ៤០. អថេរបរិស្ថាន និង dotenv
Manage configuration with environment variables.

គ្រប់គ្រងការកំណត់រចនាសម្ព័ន្ធជាមួយអថេរបរិស្ថាន។

#### Example

```javascript
require('dotenv').config();
console.log(process.env.DB_HOST);
```

#### Explanation
កូដនេះប្រើ `dotenv` ដើម្បីផ្ទុកអថេរបរិស្ថានពីឯកសារ `.env` និងបង្ហាញ `DB_HOST`។

#### Output

```text
localhost
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការប្រើ `dotenv` សម្រាប់គ្រប់គ្រងការកំណត់រចនាសម្ព័ន្ធ។

### 41. Process Management with PM2

### ៤១. ការគ្រប់គ្រងដំណើរការជាមួយ PM2
Manage Node.js processes with PM2.

គ្រប់គ្រងដំណើរការ Node.js ដោយប្រើ PM2។

#### Example

```bash
pm2 start app.js
pm2 logs
```

#### Explanation
កូដនេះប្រើ `pm2` ដើម្បីចាប់ផ្តើម `app.js` និងបង្ហាញកំណត់ហេតុ។

#### Output

```text
App logs
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ PM2 សម្រាប់គ្រប់គ្រងដំណើរការកម្មវិធី។

### 42. Deployment on Heroku / Vercel / AWS / DigitalOcean

### ៤២. ការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku / Vercel / AWS / DigitalOcean
Deploy Node.js applications to various platforms.

ដាក់ឱ្យប្រើប្រាស់កម្មវិធី Node.js នៅលើវេទិកាផ្សេងៗ។

#### Example

```bash
# Deploy to Heroku
git push heroku main
```

#### Explanation
កូដនេះបង្ហាញពីការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku ដោយប្រើ `git push`។

#### Output

```text
Deployed successfully
```

#### Summary / សរុប
ជំពូកនេះណែនាំពីការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku, Vercel, AWS, និង DigitalOcean។

### 43. CI/CD for Node.js Apps

### ៤៣. CI/CD សម្រាប់កម្មវិធី Node.js
Set up continuous integration and deployment pipelines.

រៀបចំបំពង់ CI/CD សម្រាប់កម្មវិធី Node.js។

#### Example

```yaml
# Example GitHub Actions workflow
name: CI
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: npm install
      - run: npm test
```

#### Explanation
កូដនេះជា workflow សម្រាប់ GitHub Actions ដើម្បីធ្វើ CI ដោយដំឡើង dependencies និងសាកល្បងកម្មវិធី។

#### Output

```text
CI passed
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការរៀបចំ CI/CD សម្រាប់ការអភិវឌ្ឍ និងដាក់ឱ្យប្រើប្រាស់ដោយស្វ័យប្រវត្តិ។

### 44. Dockerizing Node.js Applications

### ៤៤. ការបង្កើត Docker សម្រាប់កម្មវិធី Node.js
Containerize Node.js applications using Docker for consistent deployment.

បង្កើត container សម្រាប់កម្មវិធី Node.js ដោយប្រើ Docker ដើម្បីធានាការដាក់ឱ្យប្រើប្រាស់ប្រកបដោយភាពស៊ីសង្វាក់។

#### Example

```dockerfile
# Dockerfile
FROM node:18
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "app.js"]
```

#### Explanation
កូដនេះជា `Dockerfile` សម្រាប់បង្កើត Docker image។ វាប្រើ Node.js version 18 ជា base image, កំណត់ working directory, ដំឡើង dependencies, ចម្លងឯកសារ, បើក port 3000, និងដំណើរការ `app.js`។

#### Output

```text
Docker image built and running
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការប្រើ Docker ដើម្បីបង្កើត container សម្រាប់កម្មវិធី Node.js ដើម្បីភាពងាយស្រួលក្នុងការដាក់ឱ្យប្រើប្រាស់។

### 45. GraphQL with Node.js

### ៤៥. GraphQL ជាមួយ Node.js
Build GraphQL APIs using Node.js and Apollo Server.

អភិវឌ្ឍ GraphQL APIs ដោយប្រើ Node.js និង Apollo Server។

#### Example

```javascript
const { ApolloServer, gql } = require('apollo-server');
const typeDefs = gql`
  type Query {
    hello: String
  }
`;
const resolvers = { Query: { hello: () => 'Hello, GraphQL!' } };
const server = new ApolloServer({ typeDefs, resolvers });
server.listen(3000).then(() => console.log('Server running'));
```

#### Explanation
កូដនេះបង្កើត GraphQL server ដោយប្រើ Apollo Server។ វាកំណត់ schema ជាមួយ query `hello` និង resolver ដែលឆ្លើយតបជាមួយ 'Hello, GraphQL!'។ Server ដំណើរការនៅ port 3000។

#### Output

```text
Server running
```

#### Summary / សរុប
ជំពូកនេះណែនាំពីការបង្កើត GraphQL APIs ដោយប្រើ Apollo Server នៅក្នុង Node.js។

### 46. Microservices Architecture with Node.js

### ៤៦. ស្ថាបត្យកម្ម Microservices ជាមួយ Node.js
Design and implement microservices with Node.js.

រចនា និងអនុវត្ត microservices ជាមួយ Node.js។

#### Example

```javascript
const express = require('express');
const app = express();
app.get('/service1', (req, res) => res.json({ service: 'Service 1' }));
app.listen(3001, () => console.log('Service 1 running'));
```

#### Explanation
កូដនេះបង្កើត microservice សាមញ្ញមួយដែលដំណើរការនៅ port 3001 និងឆ្លើយតបជាមួយ JSON data។ វាអាចជាផ្នែកមួយនៃប្រព័ន្ធ microservices។

#### Output

```text
Service 1 running
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការរចនា និងអនុវត្ត microservices ដោយប្រើ Node.js សម្រាប់ប្រព័ន្ធដែលអាចពង្រីកបាន។

### 47. Building CLI Tools with Node.js

### ៤៧. ការបង្កើតឧបករណ៍ CLI ជាមួយ Node.js
Create command-line interface tools using Node.js.

បង្កើតឧបករណ៍ command-line interface ដោយប្រើ Node.js។

#### Example

```javascript
const { program } = require('commander');
program
  .command('greet <name>')
  .action((name) => console.log(`Hello, ${name}!`));
program.parse(process.argv);
```

#### Explanation
កូដនេះប្រើ `commander` ដើម្បីបង្កើត CLI tool។ ពាក្យបញ្ជា `greet` ទទួលយកឈ្មោះ និងបង្ហាញសារស្វាគមន៍។ ឧទាហរណ៍៖ `node app.js greet John`។

#### Output

```text
Hello, John!
```

#### Summary / សរុប
ជំពូកនេះបង្ហាញពីការបង្កើត CLI tools ដោយប្រើ Node.js និង `commander`។

### 48. Serverless Functions (AWS Lambda, Vercel)

### ៤៨. Serverless Functions (AWS Lambda, Vercel)
Deploy serverless functions using Node.js on platforms like AWS Lambda and Vercel.

ដាក់ឱ្យប្រើប្រាស់ serverless functions ដោយប្រើ Node.js នៅលើវេទិកាដូចជា AWS Lambda និង Vercel។

#### Example

```properties
exports.handler = async (event) => {
  return {
    statusCode: 200,
    body: JSON.stringify({ message: 'Hello from Lambda!' })
  };
};
```

#### Explanation
កូដនេះជា AWS Lambda function ដែលឆ្លើយតបជាមួយ JSON message។ វាអាចដាក់ឱ្យប្រើប្រាស់នៅលើ AWS Lambda ឬ platform serverless ផ្សេងៗ។

#### Output

```json
{ "message": "Hello from Lambda!" }
```

#### Summary / សរុប
ជំពូកនេះណែនាំពីការបង្កើត និងដាក់ឱ្យប្រើប្រាស់ serverless functions ជាមួយ Node.js។

### 49. Monorepo & Workspace Management (Nx, Turborepo)

### ៤៩. ការគ្រប់គ្រង Monorepo និង Workspace (Nx, Turborepo)
Manage multiple Node.js projects in a monorepo using Nx or Turborepo.

គ្រប់គ្រងគម្រោង Node.js ច្រើននៅក្នុង monorepo ដោយប្រើ Nx ឬ Turborepo។

#### Example

```bash
# Example Nx workspace setup
npx create-nx-workspace my-workspace
cd my-workspace
nx g @nrwl/node:app my-app
```

#### Explanation
កូដនេះបង្ហាញពីការបង្កើត Nx workspace និងបង្កើត Node.js app នៅក្នុង monorepo។ Nx ជួយគ្រប់គ្រងគម្រោងច្រើន។

#### Output

```text
Workspace and app created
```

#### Summary / សរុប
ជំពូកនេះពន្យល់ពីការប្រើ Nx ឬ Turborepo សម្រាប់គ្រប់គ្រង monorepo នៅក្នុង Node.js។

### 50. Best Practices & Node.js Project Structure

### ៥០. ការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោង Node.js
Learn best practices and recommended project structure for Node.js applications.

ស្វែងយល់អំពីការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោងដែលបានណែនាំសម្រាប់កម្មវិធី Node.js។

#### Example

```bash
# Recommended project structure
my-app/
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   └── app.js
├── tests/
├── package.json
└── .env
```

#### Explanation
កូដនេះបង្ហាញរចនាសម្ព័ន្ធគម្រោងដែលបានណែនាំ ដោយបែងចែក controllers, routes, models, និង middlewares នៅក្នុងថត `src`។

#### Output

```text
Structured project
```

#### Summary / សរុប
ជំពូកនេះផ្តល់ការណែនាំអំពីការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោងសម្រាប់កម្មវិធី Node.js។

## Additional Resources

### Official Documentation
Node.js Official Documentation
Complete official Node.js documentation
npm Documentation
Official npm package manager documentation

### Recommended Tools
Postman
API development and testing tool
ឧបករណ៍អភិវឌ្ឍ និងសាកល្បង API
MongoDB Compass
GUI for MongoDB database management
GUI សម្រាប់គ្រប់គ្រងមូលដ្ឋានទិន្នន័យ MongoDB
PM2
Production process manager for Node.js
កម្មវិធីគ្រប់គ្រងដំណើរការសម្រាប់ Node.js នៅក្នុងផលិតកម្ម
ុង Node.js។

Example
const express = require('express');
const app = express();
app.use(express.json());
app.post('/login', (req, res) => {
  const { username, password } = req.body;
  if (username === 'admin' && password === 'pass') res.json({ token: 'abc123' });
  else res.status(401).json({ error: 'Invalid credentials' });
});
app.listen(3000);
Explanation:
កូដនេះបង្កើត endpoint `/login` សម្រាប់ផ្ទៀងផ្ទាត់អ្នកប្រើ។ ប្រសិនបើ username និង password ត្រឹមត្រូវ វាផ្តល់ token។

Output:
{ "token": "abc123" }
Summary / សរុប:
ជំពូកនេះណែនាំពីគោលគំនិតនៃការផ្ទៀងផ្ទាត់អ្នកប្រើនៅក្នុង Node.js។

28. JSON Web Tokens (JWT)
២៨. JSON Web Tokens (JWT)
Implement JWT for secure authentication.

អនុវត្ត JWT សម្រាប់ការផ្ទៀងផ្ទាត់ប្រកបដោយសុវត្ថិភាព។

Example
const jwt = require('jsonwebtoken');
const token = jwt.sign({ userId: 1 }, 'secret', { expiresIn: '1h' });
console.log(token);
Explanation:
កូដនេះប្រើ `jsonwebtoken` ដើម្បីបង្កើត JWT token ដែលមាន `userId` និងផុតកំណត់ក្នុង 1 ម៉ោង។

Output:
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការប្រើ JWT សម្រាប់ការផ្ទៀងផ្ទាត់ប្រកបដោយសុវត្ថិភាព។

29. Sessions & Cookies
២៩. Sessions និង Cookies
Manage user sessions and cookies in Node.js.

គ្រប់គ្រង sessions និង cookies របស់អ្នកប្រើនៅក្នុង Node.js។

Example
const express = require('express');
const cookieParser = require('cookie-parser');
const app = express();
app.use(cookieParser());
app.get('/', (req, res) => {
  res.cookie('name', 'John');
  res.send('Cookie set');
});
app.listen(3000);
Explanation:
កូដនេះប្រើ `cookie-parser` ដើម្បីកំណត់ cookie `name` ជាមួយតម្លៃ 'John'។

Output:
Cookie set
Summary / សរុប:
ជំពូកនេះពន្យល់ពីការគ្រប់គ្រង sessions និង cookies នៅក្នុង Node.js។

30. Password Hashing (bcrypt, crypto)
៣០. ការធ្វើ Hash លើលេខសម្ងាត់ (bcrypt, crypto)
Securely hash passwords using bcrypt or crypto.

ធ្វើ hash លើលេខសម្ងាត់ប្រកបដោយសុវត្ថិភាពដោយប្រើ bcrypt ឬ crypto។

Example
const bcrypt = require('bcryptjs');
bcrypt.hash('password', 10, (err, hash) => console.log(hash));
Explanation:
កូដនេះប្រើ `bcrypt` ដើម្បីធ្វើ hash លើលេខសម្ងាត់ 'password' ជាមួយ salt rounds 10។

Output:
$2a$10$...
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការធ្វើ hash លើលេខសម្ងាត់ដើម្បីសុវត្ថិភាព។

31. Securing APIs (Helmet, Rate Limiting, CORS)
៣១. ការការពារ APIs (Helmet, Rate Limiting, CORS)
Secure APIs with Helmet, rate limiting, and CORS.

ការពារ APIs ដោយប្រើ Helmet, rate limiting, និង CORS។

Example
const express = require('express');
const helmet = require('helmet');
const app = express();
app.use(helmet());
app.get('/', (req, res) => res.send('Secure API'));
app.listen(3000);
Explanation:
កូដនេះប្រើ `helmet` ដើម្បីបន្ថែម headers សុវត្ថិភាពទៅ API។

Output:
Secure API
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការការពារ APIs ដោយប្រើឧបករណ៍ដូចជា Helmet និង CORS។

5. Advanced Node.js
Node.js កម្រិតខ្ពស់
Advanced concepts for building scalable Node.js applications.

គោលគំនិតកម្រិតខ្ពស់សម្រាប់អភិវឌ្ឍកម្មវិធី Node.js ដែលអាចពង្រីកបាន។

32. Streams & Buffers
៣២. Streams និង Buffers
Handle large data efficiently with streams and buffers.

គ្រប់គ្រងទិន្នន័យធំប្រកបដោយប្រសិទ្ធភាពជាមួយ streams និង buffers។

Example
const fs = require('fs');
const readStream = fs.createReadStream('large.txt');
readStream.on('data', (chunk) => console.log(chunk.length));
Explanation:
កូដនេះប្រើ `createReadStream` ដើម្បីអានឯកសារធំជាផ្នែកៗ (chunks) និងបង្ហាញទំហំនៃ chunk នីមួយៗ។

Output:
65536
Summary / សរុប:
ជំពូកនេះពន្យល់ពី streams និង buffers សម្រាប់គ្រប់គ្រងទិន្នន័យធំ។

33. Child Processes
៣៣. Child Processes
Run external processes using child_process module.

ដំណើរការដំណើរការខាងក្រៅដោយប្រើម៉ូឌុល child_process។

Example
const { exec } = require('child_process');
exec('ls', (err, stdout) => console.log(stdout));
Explanation:
កូដនេះប្រើ `exec` ដើម្បីដំណើរការពាក្យបញ្ជា `ls` និងបង្ហាញឈ្មោះឯកសារនៅក្នុងថត។

Output:
file1.txt
file2.txt
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការប្រើ `child_process` ដើម្បីដំណើរការពាក្យបញ្ជាខាងក្រៅ។

34. Worker Threads & Clustering
៣៤. Worker Threads និង Clustering
Scale applications using worker threads and clustering.

ពង្រីកកម្មវិធីដោយប្រើ worker threads និង clustering។

Example
const cluster = require('cluster');
if (cluster.isMaster) {
  cluster.fork();
} else {
  console.log('Worker running');
}
Explanation:
កូដនេះប្រើ `cluster` ដើម្បីបង្កើត worker process។ ប្រសិនបើជា master process វាបង្កើត worker ថ្មី។

Output:
Worker running
Summary / សរុប:
ជំពូកនេះពន្យល់ពី worker threads និង clustering សម្រាប់ការពង្រីកកម្មវិធី។

35. WebSockets & Real-Time Communication (Socket.io)
៣៥. WebSockets និងការទំនាក់ទំនងតាមពេលជាក់ស្តែង (Socket.io)
Implement real-time communication with Socket.io.

អនុវត្តការទំនាក់ទំនងតាមពេលជាក់ស្តែងជាមួយ Socket.io។

Example
const io = require('socket.io')(3000);
io.on('connection', (socket) => socket.emit('message', 'Hello!'));
Explanation:
កូដនេះបង្កើត WebSocket server ជាមួយ `socket.io` នៅ port 3000 និងផ្ញើសារ 'Hello!' ទៅ client ដែលភ្ជាប់។

Output:
Hello!
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការប្រើ Socket.io សម្រាប់ការទំនាក់ទំនងតាមពេលជាក់ស្តែង។

36. Event Loop & Async Patterns
៣៦. Event Loop និង Async Patterns
Understand the Node.js event loop and async patterns.

យល់ដឹងអំពី event loop និង async patterns នៅក្នុង Node.js។

Example
setImmediate(() => console.log('Immediate'));
setTimeout(() => console.log('Timeout'), 0);
Explanation:
កូដនេះបង្ហាញពី event loop។ `setImmediate` និង `setTimeout` ដំណើរការដោយអសមកាល ដោយ `setImmediate` មានអាទិភាពខ្ពស់ជាង។

Output:
Immediate
Timeout
Summary / សរុប:
ជំពូកនេះពន្យល់ពី event loop និងរបៀបគ្រប់គ្រងការងារអសមកាល។

37. Performance Optimization (caching, scaling)
៣៧. ការបង្កើនប្រសិទ្ធភាព (caching, scaling)
Optimize Node.js applications for performance.

បង្កើនប្រសិទ្ធភាពកម្មវិធី Node.js សម្រាប់ការអនុវត្ត។

Example
const cache = new Map();
function getData(key) {
  if (cache.has(key)) return cache.get(key);
  const data = 'Expensive operation';
  cache.set(key, data);
  return data;
}
console.log(getData('key'));
Explanation:
កូដនេះប្រើ `Map` សម្រាប់ caching ដើម្បីជៀសវាងការគណនាដែលមានតម្លៃថ្លៃ។

Output:
Expensive operation
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការបង្កើនប្រសិទ្ធភាពដោយប្រើ caching និង scaling។

38. Testing (Mocha, Jest, Supertest)
៣៨. ការធ្វើតេស្ត (Mocha, Jest, Supertest)
Test Node.js applications using Mocha, Jest, and Supertest.

ធ្វើតេស្តកម្មវិធី Node.js ដោយប្រើ Mocha, Jest, និង Supertest។

Example
const { expect } = require('chai');
describe('Math', () => {
  it('should add numbers', () => expect(1 + 1).to.equal(2));
});
Explanation:
កូដនេះប្រើ `chai` និង Mocha ដើម្បីសាកល្បងថាតើ 1 + 1 ស្មើ 2។

Output:
Test passed
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការធ្វើតេស្តកម្មវិធីដោយប្រើ Mocha, Jest, និង Supertest។

39. Debugging with Node Inspector
៣៩. ការបំបាត់កំហុសជាមួយ Node Inspector
Debug Node.js applications using Node Inspector.

បំបាត់កំហុសកម្មវិធី Node.js ដោយប្រើ Node Inspector។

Example
node --inspect app.js
// In browser: chrome://inspect
Explanation:
កូដនេះចាប់ផ្តើម `app.js` ជាមួយ `--inspect` ដើម្បីបើក Node Inspector សម្រាប់បំបាត់កំហុសនៅក្នុង Chrome។

Output:
Debugger attached
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការបំបាត់កំហុសជាមួយ Node Inspector នៅក្នុង browser។

40. Environment Variables & dotenv
៤០. អថេរបរិស្ថាន និង dotenv
Manage configuration with environment variables.

គ្រប់គ្រងការកំណត់រចនាសម្ព័ន្ធជាមួយអថេរបរិស្ថាន។

Example
require('dotenv').config();
console.log(process.env.DB_HOST);
Explanation:
កូដនេះប្រើ `dotenv` ដើម្បីផ្ទុកអថេរបរិស្ថានពីឯកសារ `.env` និងបង្ហាញ `DB_HOST`។

Output:
localhost
Summary / សរុប:
ជំពូកនេះពន្យល់ពីការប្រើ `dotenv` សម្រាប់គ្រប់គ្រងការកំណត់រចនាសម្ព័ន្ធ។

41. Process Management with PM2
៤១. ការគ្រប់គ្រងដំណើរការជាមួយ PM2
Manage Node.js processes with PM2.

គ្រប់គ្រងដំណើរការ Node.js ដោយប្រើ PM2។

Example
pm2 start app.js
pm2 logs
Explanation:
កូដនេះប្រើ `pm2` ដើម្បីចាប់ផ្តើម `app.js` និងបង្ហាញកំណត់ហេតុ។

Output:
App logs
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការប្រើ PM2 សម្រាប់គ្រប់គ្រងដំណើរការកម្មវិធី។

42. Deployment on Heroku / Vercel / AWS / DigitalOcean
៤២. ការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku / Vercel / AWS / DigitalOcean
Deploy Node.js applications to various platforms.

ដាក់ឱ្យប្រើប្រាស់កម្មវិធី Node.js នៅលើវេទិកាផ្សេងៗ។

Example
# Deploy to Heroku
git push heroku main
Explanation:
កូដនេះបង្ហាញពីការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku ដោយប្រើ `git push`។

Output:
Deployed successfully
Summary / សរុប:
ជំពូកនេះណែនាំពីការដាក់ឱ្យប្រើប្រាស់នៅលើ Heroku, Vercel, AWS, និង DigitalOcean។

43. CI/CD for Node.js Apps
៤៣. CI/CD សម្រាប់កម្មវិធី Node.js
Set up continuous integration and deployment pipelines.

រៀបចំបំពង់ CI/CD សម្រាប់កម្មវិធី Node.js។

Example
# Example GitHub Actions workflow
name: CI
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: npm install
      - run: npm test
Explanation:
កូដនេះជា workflow សម្រាប់ GitHub Actions ដើម្បីធ្វើ CI ដោយដំឡើង dependencies និងសាកល្បងកម្មវិធី។

Output:
CI passed
Summary / សរុប:
ជំពូកនេះពន្យល់ពីការរៀបចំ CI/CD សម្រាប់ការអភិវឌ្ឍ និងដាក់ឱ្យប្រើប្រាស់ដោយស្វ័យប្រវត្តិ។

44. Dockerizing Node.js Applications
៤៤. ការបង្កើត Docker សម្រាប់កម្មវិធី Node.js
Containerize Node.js applications using Docker for consistent deployment.

បង្កើត container សម្រាប់កម្មវិធី Node.js ដោយប្រើ Docker ដើម្បីធានាការដាក់ឱ្យប្រើប្រាស់ប្រកបដោយភាពស៊ីសង្វាក់។

Example
# Dockerfile
FROM node:18
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "app.js"]
Explanation:
កូដនេះជា `Dockerfile` សម្រាប់បង្កើត Docker image។ វាប្រើ Node.js version 18 ជា base image, កំណត់ working directory, ដំឡើង dependencies, ចម្លងឯកសារ, បើក port 3000, និងដំណើរការ `app.js`។

Output:
Docker image built and running
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការប្រើ Docker ដើម្បីបង្កើត container សម្រាប់កម្មវិធី Node.js ដើម្បីភាពងាយស្រួលក្នុងការដាក់ឱ្យប្រើប្រាស់។

45. GraphQL with Node.js
៤៥. GraphQL ជាមួយ Node.js
Build GraphQL APIs using Node.js and Apollo Server.

អភិវឌ្ឍ GraphQL APIs ដោយប្រើ Node.js និង Apollo Server។

Example
const { ApolloServer, gql } = require('apollo-server');
const typeDefs = gql`
  type Query {
    hello: String
  }
`;
const resolvers = { Query: { hello: () => 'Hello, GraphQL!' } };
const server = new ApolloServer({ typeDefs, resolvers });
server.listen(3000).then(() => console.log('Server running'));
Explanation:
កូដនេះបង្កើត GraphQL server ដោយប្រើ Apollo Server។ វាកំណត់ schema ជាមួយ query `hello` និង resolver ដែលឆ្លើយតបជាមួយ 'Hello, GraphQL!'។ Server ដំណើរការនៅ port 3000។

Output:
Server running
Summary / សរុប:
ជំពូកនេះណែនាំពីការបង្កើត GraphQL APIs ដោយប្រើ Apollo Server នៅក្នុង Node.js។

46. Microservices Architecture with Node.js
៤៦. ស្ថាបត្យកម្ម Microservices ជាមួយ Node.js
Design and implement microservices with Node.js.

រចនា និងអនុវត្ត microservices ជាមួយ Node.js។

Example
const express = require('express');
const app = express();
app.get('/service1', (req, res) => res.json({ service: 'Service 1' }));
app.listen(3001, () => console.log('Service 1 running'));
Explanation:
កូដនេះបង្កើត microservice សាមញ្ញមួយដែលដំណើរការនៅ port 3001 និងឆ្លើយតបជាមួយ JSON data។ វាអាចជាផ្នែកមួយនៃប្រព័ន្ធ microservices។

Output:
Service 1 running
Summary / សរុប:
ជំពូកនេះពន្យល់ពីការរចនា និងអនុវត្ត microservices ដោយប្រើ Node.js សម្រាប់ប្រព័ន្ធដែលអាចពង្រីកបាន។

47. Building CLI Tools with Node.js
៤៧. ការបង្កើតឧបករណ៍ CLI ជាមួយ Node.js
Create command-line interface tools using Node.js.

បង្កើតឧបករណ៍ command-line interface ដោយប្រើ Node.js។

Example
const { program } = require('commander');
program
  .command('greet <name>')
  .action((name) => console.log(`Hello, ${name}!`));
program.parse(process.argv);
Explanation:
កូដនេះប្រើ `commander` ដើម្បីបង្កើត CLI tool។ ពាក្យបញ្ជា `greet` ទទួលយកឈ្មោះ និងបង្ហាញសារស្វាគមន៍។ ឧទាហរណ៍៖ `node app.js greet John`។

Output:
Hello, John!
Summary / សរុប:
ជំពូកនេះបង្ហាញពីការបង្កើត CLI tools ដោយប្រើ Node.js និង `commander`។

48. Serverless Functions (AWS Lambda, Vercel)
៤៨. Serverless Functions (AWS Lambda, Vercel)
Deploy serverless functions using Node.js on platforms like AWS Lambda and Vercel.

ដាក់ឱ្យប្រើប្រាស់ serverless functions ដោយប្រើ Node.js នៅលើវេទិកាដូចជា AWS Lambda និង Vercel។

Example
exports.handler = async (event) => {
  return {
    statusCode: 200,
    body: JSON.stringify({ message: 'Hello from Lambda!' })
  };
};
Explanation:
កូដនេះជា AWS Lambda function ដែលឆ្លើយតបជាមួយ JSON message។ វាអាចដាក់ឱ្យប្រើប្រាស់នៅលើ AWS Lambda ឬ platform serverless ផ្សេងៗ។

Output:
{ "message": "Hello from Lambda!" }
Summary / សរុប:
ជំពូកនេះណែនាំពីការបង្កើត និងដាក់ឱ្យប្រើប្រាស់ serverless functions ជាមួយ Node.js។

49. Monorepo & Workspace Management (Nx, Turborepo)
៤៩. ការគ្រប់គ្រង Monorepo និង Workspace (Nx, Turborepo)
Manage multiple Node.js projects in a monorepo using Nx or Turborepo.

គ្រប់គ្រងគម្រោង Node.js ច្រើននៅក្នុង monorepo ដោយប្រើ Nx ឬ Turborepo។

Example
# Example Nx workspace setup
npx create-nx-workspace my-workspace
cd my-workspace
nx g @nrwl/node:app my-app
Explanation:
កូដនេះបង្ហាញពីការបង្កើត Nx workspace និងបង្កើត Node.js app នៅក្នុង monorepo។ Nx ជួយគ្រប់គ្រងគម្រោងច្រើន។

Output:
Workspace and app created
Summary / សរុប:
ជំពូកនេះពន្យល់ពីការប្រើ Nx ឬ Turborepo សម្រាប់គ្រប់គ្រង monorepo នៅក្នុង Node.js។

50. Best Practices & Node.js Project Structure
៥០. ការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោង Node.js
Learn best practices and recommended project structure for Node.js applications.

ស្វែងយល់អំពីការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោងដែលបានណែនាំសម្រាប់កម្មវិធី Node.js។

Example
# Recommended project structure
my-app/
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   └── app.js
├── tests/
├── package.json
└── .env
Explanation:
កូដនេះបង្ហាញរចនាសម្ព័ន្ធគម្រោងដែលបានណែនាំ ដោយបែងចែក controllers, routes, models, និង middlewares នៅក្នុងថត `src`។

Output:
Structured project
Summary / សរុប:
ជំពូកនេះផ្តល់ការណែនាំអំពីការអនុវត្តល្អបំផុត និងរចនាសម្ព័ន្ធគម្រោងសម្រាប់កម្មវិធី Node.js។

Additional Resources
Official Documentation
Node.js Official Documentation
Complete official Node.js documentation
npm Documentation
Official npm package manager documentation
Recommended Tools
Postman
API development and testing tool
ឧបករណ៍អភិវឌ្ឍ និងសាកល្បង API
MongoDB Compass
GUI for MongoDB database management
GUI សម្រាប់គ្រប់គ្រងមូលដ្ឋានទិន្នន័យ MongoDB
PM2
Production process manager for Node.js
កម្មវិធីគ្រប់គ្រងដំណើរការសម្រាប់ Node.js នៅក្នុងផលិតកម្ម