# tm.pagination
angular分页插件tm.pagination（解决触发二次请求的问题）
根据条件查询
需要重新定义一个方法列：
$scope.so = function () {
            if ($scope.paginationConf.currentPage != 1) {
                $scope.paginationConf.currentPage = 1;
            }else{
                $scope.poat();
            }
}
原因：解决了二次请求的问题，但是回归第一页需要重新赋值为1才行

