var express = require('express'),
	app = express();
  app.use(express.static(__dirname + '/public'));
app.set('views', __dirname + '/views');
var expressHbs = require('express3-handlebars');
app.engine('hbs', expressHbs({extname:'hbs'}));
app.set('view engine', 'hbs');

var router = express.Router();
var fs = require('fs');
var server = app.listen(3000,function(){
	console.log("Listening");
});
var clients = [];
app.use(express.static('public'));
app.get('/',function(req,res){
	res.send("home");
});
app.get('/teacher',function(req,res){
	res.send("teacher");
});
app.get('/student',function(req,res){
	res.send('student');
});
app.get('/video',function(req,res){
	res.send('video_stream');
});

