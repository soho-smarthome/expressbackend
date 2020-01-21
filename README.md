1. 安装express
   npm install express  -g
   npm install express-generator -g
   
   express --version
   
   express expressbackend

2. 安装好mongodb后，添加测试数据，或者通过postman添加
 mongoimport -d test -c products products.json
 mongoimport -d test -c products manufacturers.json
 
3. http://localhost:3000/api/v1/manufacturers  GET POST PUT DELETE
   {
	  "name": "小米"
   }

   http://localhost:3000/api/v1/products   GET POST PUT DELETE
   {
		"name": "Mix Alpha",
		"description": "这个哪一款小米手机呢",
		"image": "http://oss.aliyun.com/1.jpg",
		"price": 1999,
		"manufacturer": "5e2415763683c069e8cfbaa4"
   }