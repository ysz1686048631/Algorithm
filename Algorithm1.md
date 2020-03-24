 1.  取出字符串中数字 

     var str = ' ab-12343109cwhen open';

​     function getnum(str){

​          str = str.replace(/\s+/g,'');

​        var len = str.length; 

​        var sum = ''; 

​          for(let i = 0;i<len;i++){

​            console.log();

​            if(str[i].charCodeAt()<97){

​               sum+=str[i];  

​            }

​          }

​          return parseInt(sum);

​     }

​     

​    //  console.log(getnum(str))  
```

 2.获取公共字母

​      var arr = ['flower','fowe','flowringj'];

​        function gettong(arr){

​          let len = arr.length;

​          let first = arr[0];

​          var firstStr='';

​          for(let i = 0;i<first.length;){

​            // 让所有的数组元素都与第一个元素匹配 

​             firstStr = first.substring(0,i); //随匹配成功字符串加长

​             for(let a = 1;a<len;a++){

​                  

​                  if(arr[a].indexOf(firstStr)==0){

​                    //  每次判断是否存在 并且 是否循环到最后

​                     if(a==len-1){

​                       i++;

​                      }

​                  }else{

​                    // 这里不用担心 中间元素是否存在指定字符串 如果不存在直接停止                   返回结果

​                    return first.substring(0,i-1);

​                  }

​              }

​          }

​               

​          

​        } 

​        console.log(gettong(arr));