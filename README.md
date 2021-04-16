# Ricky's Prototype e-commerce B2C online website

## 1. Software Requirements
- NPM version 6.14.4 above (Package Manager)
- Node JS version 10.19.0 above (Runtime Environment)
- Windows 10 OS, or Mac OS with version 10.14 or later

## 2. Setup
### 2.1 Before Start
Download the source code in this repository and run below command under the root directory to install the dependency.

```
npm install
```

### 2.2 Backend Application

server.js is the entry point the backend application, other backend related coding logic is placed under folder `server/`

Start the backend application with the command below.
```
node server.js
```

### 2.3 Frontend Application

All the frontend coding logic is placed under the folder `src/`

Start the frontend application in development mode with the command below
```
npm run start
```
Goto http://localhost:3000/ through web browser, you should see a store website now.

### 2.4 Database

A SQLite file-based database named `shop.db` is placed under `server/db/` folder. You are expected to use the provided client based on your OS (Window 10, MacOS) to connect to the database by executing below command

Window
```
server/db/sqlite3-window
```

MacOS
```
server/db/sqlite3-macos
```

To open the provided database in the CLI
```
> .open shop.db
```

| command | description |
| ------ | ------ |
| .table | List the existing table in databse after connected |
| .schema {Table} | Look up the table schema |

Note that you may need to search other necessary commands for the assessment.

A product will be treated as **OBSOLETED** when the `type` is **B** and `price` is higher than **$20** at this moment.

Shopping cart page (http://localhost:3000/cart).
