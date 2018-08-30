# 转义符转化为普通html标签
        
        function escape2Html(str) {
            var arrEntities={'lt':'<','gt':'>','nbsp':' ','amp':'&','quot':'"','hellip':'…','mdash':'—'};
            return str.replace(/&(lt|gt|nbsp|amp|quot|hellip|mdash);/ig,function(all,t){return arrEntities[t];});
        }
