const express = require('express');

const app = express()

app.get("/Home",(req,res)=>{

    res.send("<h1>Hello Welcome To My Page</h1>");


})

app.get("/about",(req,res)=>{

    res.send({
        Name:"JAMES",
        Hobby:"Learning"
    })
})

app.get("/Vision",(req,res)=>{
    res.send("<h1>U Can Know About Us Well</h1>");
})


app.get("",(req,res)=>{
    res.send("<h1>U Are Now Looking About Your Future</h1>")
})




app.listen(3000,()=>{

    console.log('Server Starting Uo At:3000;');
})
