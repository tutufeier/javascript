# js-basic
js small programs

## 进制转换方法一
var str = '0xCAFE911';
var arr = str.split('').reverse();
var i ,j=0,transnum=0;

for(i=0; i<parseInt(str.length-2);i++){
	transnum += parseInt(arr[i],16) * Math.pow(16, j);
	j++;
}

console.log(transnum);
