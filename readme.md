How do we Use it 
-------
Working as a frontend engineer and building a dummy or proof-of-concept project without a complete backend might be very challenging to set up REST API’s. 
You can use Firebase or many other things to setup backend without writing much code. BUT,
There is a way to set up an incredibly simple backend server running on your localhost. 
It will be a Node project.
Let’s assume you have a frontend, we can create a backend server using an NPM module json-server.
Let name your node project “FakeBackend”.

**Steps:**

- Make a directory FakeBackend
- cd FakeBackend
- npm init
- Follow the setup CLI by providing basics info for you Node project
- npm install json-server -g
- Make a db.json file. Run touch db.json
- You need to watch that file
- In package.json write a start script as => json-server -p 3007 -w db.json
- Put your JSON in db.json
- npm start

That is all you have to do if you want to set up a fake backend server :)

**Making an API call from POSTMAN**

**GET ::: localhost:3007/profile**
```
{
  "name": "yogendra",
  "age": 25,
  "country": "INDIA",
  "profession": "Engineer"
}
```

If you make a POST call, then data will automatically get updated in db.json.

**Fork, Star and contribute**

## How to Run
```
npm install
npm start
or
npx json-server -p 3007 -w db.json
```

## Author
Yogendra Saxena
