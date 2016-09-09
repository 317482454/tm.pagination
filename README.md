# tm.pagination
angular分页插件tm.pagination（解决触发二次请求的问题）<br/>
根据条件查询<br/>
需要重新定义一个方法<br/>  
```javascript
$scope.so = function () {
            if ($scope.paginationConf.currentPage != 1) {<br/>  
                $scope.paginationConf.currentPage = 1; <br/>    
            }else{<br/>    
                $scope.poat();<br/>  
            }<br/>   
}  
```
原因：解决了二次请求的问题，但是回归第一页需要重新赋值为1才行  

