const express = require ("express");

const app = express()

const port = 8000


app.get("", (req,res) =>{
   res.sendFile(__dirname + "/one/Homepage.html");
    })

app.get("/about", (req,res) => {
    res.sendFile(__dirname + "/one/about.html");
     })

app.get("/history", (req,res) =>{
        res.sendFile(__dirname + "/one/history.html");
         })

 app.get("/nani", (req,res) =>{
            res.sendFile(__dirname + "/one/nani.html");
             })


app.listen(port, () => console.info(`Listening on port ${port}`) );

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Homepage</title>
</head>
<body style="background-color:powderblue; ">
    
    <h1> Welcome from homepage</h1>
    <p> <a href="http://localhost:8000/about">about</a>
        <a href="http://localhost:8000/history">sample</a>
        <a href="http://localhost:8000/nani">project</a></p>
        <img src="../img/welcome.jpg" alt="welcome" style="width:auto;">
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Something</title>
</head>
<body style=" background-color: powderblue;">
    <h1> Ths is our project</h1>
    <p> <a href="http://localhost:8000/about">about</a>
        <a href="http://localhost:8000/history">sample</a>
        <a href="http://localhost:8000"> homepage</a></p>
        <img src="../img/project.png" alt="about" style="width:auto;">
    
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
</head>
<body style="background-color:powderblue; ">
    <h1> This is about us. </h1>
   <p> <a href="http://localhost:8000"> homepage</a>
        <a href="http://localhost:8000/history">sample</a> 
        <a href="http://localhost:8000/nani">project</a></p>
        <img src="../img/about.jpg" alt="about" style="width:auto;">
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sample</title>
</head>
<body style="background-color:powderblue; ">
    <h1>This is one of our designs.</h1>
    <p> <a href="http://localhost:8000/about"> about</a>
        <a href="http://localhost:8000/nani">project</a>
        <a href="http://localhost:8000">homepage</a></p>
        <img src="../img/design.jpg" alt="about" style="width:auto;">
</body>
</html>
