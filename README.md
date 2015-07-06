# WebSQL
Web SQL Demo

var db = openDatabase('rkdb','1.0','rkfirstdb','2*1024*1024');
db.transaction(function(tx){
	tx.executeSql("CREATE TABLE IF NOT EXISTS user(id INTEGER UNIQUE, name TEXT(100))");
	tx.executeSql("INSERT INTO user(id,name) VALUES(1,'Ranjit kumar')");
});


