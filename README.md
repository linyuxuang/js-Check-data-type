# js-Check-data-type
js 检查(原始值,数组，包装类，对象)



              function type(target){
                var ret=typeof(target);
                var template={
                  "[object Array]":'object -array',
                  "[object Object]":'object-object',
                  "[object String]":'object-string',
                  "[object Boolean]":'boolean-object',
                  "[object Number]":"object-number"
                }
                if(target==null){
                  return "null"
                }
                if(ret=="object"){
                 var str=Object.prototype.toString.call(target)
                       return template[str]			
                }else{
                  return ret
                }
               }
