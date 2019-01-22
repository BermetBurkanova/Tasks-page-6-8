# Tasks-page-6-end
# task 1
for (var i = 0; i < 10; i++) {
    setTimeout(function() {
        console.log(i);
    }
}
# Что выведет консоль и почему? Nothing is going to happens, since there is a SyntaxError. We have to put ',)' right after 'console.log(i);}' then it will work 

# task 2
var today = new Date();
  var day = today.getDay();
  var daylist = ["Sunday","Monday","Tuesday","Wednesday ","Thursday","Friday","Saturday"];
  console.log("Today is : " + daylist[day] + ".");
  var hour = today.getHours();
  var minute = today.getMinutes();
  var second = today.getSeconds();
  var prepand = (hour >= 12)? " PM ":" AM ";
  hour = (hour >= 12)? hour - 12: hour;
  if (hour===0 && prepand===' PM ') 
  { 
  if (minute===0 && second===0)
  { 
  hour=12;
  prepand=' Noon';
  } 
  else
  { 
  hour=12;
  prepand=' PM';
  } 
  } 
  if (hour===0 && prepand===' AM ') 
  { 
  if (minute===0 && second===0)
  { 
  hour=12;
  prepand=' Midnight';
  } 
  else
  { 
  hour=12;
  prepand=' AM';
  } 
  } 
console.log("Current Time : "+hour + prepand + " : " + minute + " : " + second);
# 
function reverse_n (num) {
	num = num + "";
	return num.split("").reverse().join("");
}

# 
function factorial_n (x) { 

  if (x === 0) {
    return 1;
 }
  return x * factorial_n(x-1);        
}
#
function max_n(num1 , num2){

if( num1 >= num2)
return num1;
return num2;
}
#
function myColor (arr){
myColor = arr.toString("");
myColor = arr.join("+");}
#
var get_month = function(dt){
mlist = [ "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December" ];
  return mlist[dt.getMonth()];
};
#var word = "Any";
console.log( word[0] === word[0].toUpperCase() );
# 
var canvas = document.getElementById('canvas');
var ctx = canvas.getContext('2d');

ctx.beginPath();
//arc(x,y,r,sAngle,eAngle,counterclockwise);
ctx.arc(75, 75, 50, 0, Math.PI * 2, true); // Outer circle
ctx.moveTo(110, 75);
ctx.arc(75, 75, 35, 0, Math.PI, false); // Mouth (clockwise)
ctx.moveTo(65, 65);
ctx.arc(60, 65, 5, 0, Math.PI * 2, true); // Left eye
ctx.moveTo(95, 65);
ctx.arc(90, 65, 5, 0, Math.PI * 2, true); // Right eye
ctx.stroke();
