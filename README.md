#  API Testing with Mock server
### In this project i enhanced my expertise in API testing by:
#### Developed a Mock Server:
Utilized [Json-server](https://www.npmjs.com/package/json-server) and [Json-server-auth](https://www.npmjs.com/package/json-server-auth) to create a mock server with mock APIs to replicate various endpoints and responses, simulating real-world API behavior for testing purposes.
#### Comprehensive API Testing:
Conducted API tests by exploring various scenarios and E2E tests through hands-on practice with variables, test scripts and implementing assertions to validate responses and ensure reliability.
#### Manual Execution:
Executed API collections manually using [Postman](https://www.postman.com/downloads/).
#### Automated Execution:
Automated API collection execution using [Newman](https://www.npmjs.com/package/newman) for efficiency and consistency.
#### Reporting:
Generated HTML report using [Newman-reporter-htmlextra](https://www.npmjs.com/package/newman-reporter-htmlextra) summarizing the results of the automated collection runs for better analysis and documentation.
## Preconditions
- Having [node.js](https://nodejs.org/en/download).

## To run the mock server
- Clone this directory.
- open it with VS code /or/ use any terminal.
- Move to the file path.
```
cd "write File_path or drag it and drop here"
```
- Install json-server globally
```
npm install -g json-server
```
- Install json-server-auth
```
npm install json-server json-server-auth
```
- Run your mock server
```
node server.js
```
- Modify db.json file with any json data you want.
```
{
  "Courses": [],
  "Users": []
}
```

**✨ Now you have your own server, database, and APIs, it’s time to embark on your journey—explore, innovate, and transform your ideas into reality. ✨**
## Newman commands
- **At first Open your terminal**.
- **Then git to the file path where collection and environment exist**.
```
cd "write File_path or drag it and drop here"
```
- **Running a collection**
```
newman run <Collection-file.json> -e <Environment-file.json>
EX: newman run E2E_Tests.json -e Test_env.json
```
- **Running a collection with multiple iterations**
```
newman run <Collection-file.json> -e <Environment-file.json> --iteration-count <number-of-iterations>
```
- **Running a collection with a delay between requests**
```
newman run <Collection-file.json> -e <Environment-file.json> --delay-request <delay-in-milliseconds>

```
- **Running a collection with an html report summarizing results**
```
```
 **ensure that the reporter is installed in the same directory as newman**

- npm install -g newman-reporter-htmlextra
newman run <Collection-file.json> -e <Environment-file.json> -r htmlexta

Special Thanks To Mohamed Samir
