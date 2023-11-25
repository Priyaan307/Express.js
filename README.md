# Express.js
-This is documentation of my Day38(25 Nov, 2023) of 100DaysOfCode

-Routing: Routes banane ke process ko routing kehte hain.

google.com/
http://localhost:3000/
http://localhost:3000/profile

-middleware: ek aisa function hota hai jo har route se pahle chalta hai, iska matlab saare routes mein se koi bhi chale usse pahle middleware chalta hai and usmein likha code pahle execute hota hai.

- control aagar ek baar bhi kisi middleware par gaya to control khud se agle route/middleware par nhi jaayega, usko agle par bhejne ke liye hame push karna padta hai aur ye push hi next hoti hai.

- Request and Response:

req mein saara data hota hai aane wale user ke request ki taraf se, jaise ki uski location, device info and other things, res mein controls hota hai jinke basis per hum server se response bhej pate hain, next is just a push so that our request moves to the next thing which should be executed 

- route parameters: 
dynamic routing- aaisa koi bhi route jiska koi hissa baar-2 same rehta hai aur kuch hissa baar-2 change hota hai iske liye ham dynamic route bana sakte hain.

url example:
facebook.com/profile/priya
facebook.com/profile/priyaan307
facebook.com/profile/priyanka
facebook.com/profile/priyadarshani

/profile/:username => params(colon wali  value ko kehte hain)

- to make any route dynamic we can use ':'(colon) at the place where we want to make it dynamic and to access there value use req.params

ex: facebook.com/profile/:username

- ejs is html with superpower

ejs setup steps:

1.ejs install: npm i ejs
2. configure ejs: app.set('view engine', 'ejs');
3. create a views folder
4. create ejs in the folder views
5. render in place of send => render karte time make sure views ke ander wali hi koi file ka naam likha jaye aur render function me .ejs mention na kiya jaye.

- template engines(pug, handlebars, ejs, jade) => ye ek style of markup se convert karke hame html dete hain => ejs is very very similar to html 

=> ek markup style jo baad me convert ho jayegi html me.

- static files setup steps: 

1. Create a folder called public
2. create three folders inside it, images,stylesheets,javascripts
3. configure the express static in script.js file
4. understand the path

- Error Handling: