# async

第一步：npm init -y
第二部： 创建public文件夹里面有index.html文件，在根目录创建server.js
第三步：终端下载express,与noodmon npm i express npm i noodmon -g
第四步：server.js创建服务
const express=require("express")
const app=express()
app.use(express.static("public"))
app.listen(3000,()=>{console.log("server has running")})
第五步： noodmon server.js


#总结：
处理异步的方式  
new Promise((resolve,reject)=>{})
  .then(res=>{
    new Promise((resolve,reject)=>{})
      .then(res=>{
      
      })
  })
  .catch(error=>{
    console.log(error)
  })
  使用Async则可以取消以上的then地狱回调
  
