1. 素数1

  ```
  //             var i, j, arr = [] ;
  // // 1-101 被除数
  // for( i =2; i < 101; i++) {
  // // 除数 ，因为是素数，所以从2 开始，并小于被除数, 循环
  // for( j = 2; j < i; j++) {
  // // 取模：如果能整除，表示非素数，跳出循环； 
  // if ( i % j === 0 ) {
  // break;
  // } 
  // }
  // // 放到数组里面存起
  // if (i === j ) { 
  // arr.push(i);
  // }
  // }
  // console.log ( arr);
  ```

  

3. 盛最多水的容器

```
3. // var arr = [1,2,6,2,5,4,8,3,7];
   // function warter(arr){
   //           if(arr.length<2){
   //               return 0;
   //           }
   //           let len = parseInt(arr.length/2);
      //           let left = 0;
      //           let right = arr.length-1;
             
   
   //           for(let i =0;i<len;i++){
   //                if(arr[left]<arr[i+1]){
   //                     left = i+1
   //                } 
   //           }
   //           if(arr[left]-arr[right]>0){
   //               return arr[right]*(arr.length-(left+1));
   //           }else{
   //               return arr[left]*(arr.length-(left+1));
   //           }
   // }
   // console.log(warter(arr));
   ```
   
   

4. 将整数转化位罗马数字

  ```
  // var intToRoman = function(num) {
  //     var Q = ["", "M", "MM", "MMM"];
  //     var B = ["", "C", "CC", "CCC", "CD", "D", "DC", "DCC", "DCCC", "CM"];
  //     var S = ["", "X", "XX", "XXX", "XL", "L", "LX", "LXX", "LXXX", "XC"];
  //     var G = ["", "I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX"];
  //     return Q[Math.floor(num/1000)] + B[Math.floor((num%1000)/100)] + S[Math.floor((num%100)/10)] + G[num%10];
  // };
  // console.log(intToRoman(31));
  ```

  

5. 搜索插入   题意的是 输入一个数组和一个数 判断数是否存在 如果存在就直接返回位置  不存在直接放进数组并返回位置

   ```
   4. // var searchInsert = function(nums, target) {
           
   
   //         if(nums.indexOf(target)>0){
   //             nums = nums.sort();
   //             return nums.indexOf(target);
   
   //             // return nums.indexOf(target);
   //         }  else{
   //             nums.push(target);
   //             nums = nums.sort();
   //             return nums.indexOf(target);
   //         }
   // };
   // console.log(searchInsert([1,3,4,6],7));
   ```
   
   

6.按摩师

```
// var massage = function(nums) {
//         let all = 0;
//         for(let a = 0;a<nums.length;){
//                         if(a%2==0){
//                             all+=nums[a] 
//                             if(nums[nums.length-1]>nums[a]&&a==nums.length-2&&nums.length%2==0){
//                                     all = all+nums[nums.length-1]-nums[a];
//                              }
//                     }     
//              a++;   
//         }
//         return all;
// };
```

console.log(massage([2,7,9,3,1]))