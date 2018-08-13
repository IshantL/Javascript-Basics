"# Javascript-Basics"
--Basic understanding of javascript from Beginner to pro..

onclick=""
document.getElementByID("").innerHTML="new Update";

.innerHtml is property
.src
.style.display='' etc.
for performance issue we should write script in body so that the page get load first.
---
How to see the output?
window.alert();
document.write();--comlete html loaded 
innerHTML;
console.log()
---
In this session, we are going to go over the syntax of javascript - Get to know the language better
fixed value- literal
variable valuue
expersion is a combinationof values,,variables and operatotrs
identifiers are names
JS identifier are case Sensitive
type operator:type of ,,instanceOf

Datatypes-Number,String,Array,Object,Boolean,Undefined.

scope is block scope in function.
this means in context of same.
events-onclick, onchange,onmouseover,onmouseout,onkeydown,onload

String methods
.length
.indexOf(''); position
.lastIndexOf('');
.search('');


//extractions
slice(start,end);
//apple, Banana
//slice(7,13);//banana
//slice(-13,-8);//apple

substring(start,end);
same as slice but not accept -ve values

substr(start,length)

.replace('','');
.replace('/string/g','');--to replace it at al instance
as string is imutable so it will not change the string.

.toLowerCase();
.toUpperCase();
.concat()//.concat(" ",str)-for space
+

//extracting String characters
.charAt(0);
.charCodeAt(0);//gives ascii code

split- gives output in array of string
.split(',') //based on comma
.split(' ')// based on space // we can split based on alphabet
.split('');//for empty gives complete string in array.


Numbers
var x=34;
x=34.0;
x=123e5;//12300000
x=123e-5;//0.0123
IEEE 754 -64 bit format -double presision,
0-51 ---number
1-> 00000....01

52-62 ---exponent
63---sign

upto 15 digit decimal it is appropriate aftre then abrupt behavior
upto 17 digit floting


//how to aviod such abstrupt behavior--- maths logic- we can do
//Bianary -2
//Hexadecimal-16
//octal-8
//Decimal -10

coversion 
.toString(2)//binary
.toString(8)//octal
.toString(10)//decimal

//Infinity,-Infinity-->(1/0)
//NaN--100/"hundread"
to check isNaN();
type of NAN is number;
//Number can also be Objects.


//Number Methods
.toString()//to convert no in string
(123).toString();

//toExponential()

.toExponential(parameter for round of);

//to Fixed(parameter for round of)
to rounding of the nos.

//toPrecision(length<21)

//valueOf()
to convert a number object to premitive value.

//converting variables to nos
//Number()
global js methods 
Number(true)//1
Number("10")//10
Number("djhd")//NaN

//parseInt()
parseInt("10 20")//10
//"10 years"-->10
//true-->NaN
//"years 10"-->NaN

same with parseFloat();

//Number Properties
Number.MAX_VALUE-->1.79e+308
Number.MIN_VALUE-->5e-324
Number.NEGATIVE_INFINITY
Number.POSITIVE_INFINITY

//Math object
Math.PI()
Math.round()
Math.pow(2,3);//8
Math.sqrt(64);//8
Math.abs(-4.7)//4.7
Math.ceil(4.4)//5
Math.floor(4.9)//4
Math.sin();
Math.cos();
//range -1 to 1
//Angle in radient =Angle in degree*PI/180;
Math.min(2,3,4,5,6);//2
Math.max(2,3,4,5,6);//6
Math.random()//0 to 1
Math.PI;
Math.E-euler's Number
Math.SQRT//default sqrt of 2
Math.SQRT1_2//sqrt of 1/2
Math.LN2-log2
Math.LN10//log 10
Math.LOG2E//Log E to base 2
Math.LOG10E//Log E to base 10

Math.random()

//Date Object
create a new date
new Date();
new Date(148145454545);//from 11 jan 1970 miillisecond
new Date('12/31/2016');
new Date(2016,11,31,12,30);
//years,months(0-11),days,hours,min,seconds,milliseconds)
toUTCString();
.toDateString();

new Date('2016-03-25');
//shortage Date-mm/dd/yyyy
new Date('12/31/2016');

//long dates
new Date("Mar 25 2016);

//Date Methods:
.getDate();
.getDay()//1-7
.getFullYear();//2018
.getHours();//16
.getTime()//1351564654654(ms)
.setDate();
.setYear();
.setTime(ms);
.setFullYear(2020,0,10);
//Parsing
Date.parse('Dec 31, 2016');

//Compare Dates

//Arrays

.push();
.sort()
isArray();
instanceof;

//Array Methods
.toString();
.join('')//|,etc
.push();
.pop()

//shift and unshift
//.shift()---removes the 1st element
//.unshift()---adding the 1st element

//delete
delete fruits[0];
//delete it and place undefined

//Splice- to add 2 elemebnts
fruits.splice(2//after the element,0//to remove element,'Lemon','kiwi');

//to remove
fruits.splice(0,1);

//join 
.concat();
array1.concat(array2,array3);

//to slice the array element into different array
.slice(1//index from new array formed);
.slice(1,3)//not included index

//Sorting-IMP
.sort();
.reverse();
//sort cannot use on numbers
for that we use compare
e.g var points=[40,50,100,25,10]
points.sort(function(a,b){return a-b});
//40,100 it gives 40-100=-60
therefore it keep 
//100,40
for decending
points.sort(function(a,b){return b-a});

//to sort object
var cars=[
{name:'volvo',year:2015},
{name:'Merc',year:2014},
{name:'BMW',year:2013}
]
cars.sort(function(a,b){return a.year-b.year});
console.log(cars);

//Boollean
//All real values will return true
Boolean(-4);//true
Boolean(8);//true
Boolean("ghhg");//true

//All non real values will return false
Boolean(0);//false
Boolean("");//false
Boolean(undefined);//false
Boolean(null);//false

//OBJECTS

in JS everything is objects
//Booleans
//Numbers
//stringss
//Dates
//Maths
//Regular Expresssions
//Arrays
//Functions
//objects

//premitives in JS
//string
//boolean
//number
//null
//undefined

3 ways of creating an object

//object literal
var aaa={fn:"ishant,
	ln:"lambhate"};
//new keyword

var aaa=new Object();
aaa.fn="ishant";
aaa.ln="lambhate";
//constructor

function aaa(fn,ln){
this.fn=fn;
this.ln=ln;
}

// this keyword is an object that owns the javascript code (context).


//object property
//add,change,delete
objectName.property//person.fn;
objectName['property']//person['fn'];
objectName[expression];//var x="age";person[x];

to access the property
var text="";
for(y in person){
text+=person[y];
text+="";
}

//to delete
delete person.age
//only for object property,,not used for predefined js property.
value is one of the property attribute


//objects Methods
//methodName:function(){codelines}
//objectName.methodName();
//we cannot add a method on the fly ..we can create it with literals or consuructor

//Object Prototype
every object inherit the methods etc from prototype
godfather

//object creted from literal or consructor will inherit from object.prototype();
//new Date()- Date.prototype

//we can create our own prototype

function Person(first,last,age,eyecolor){
this.fn=first;
this.ln=last;
this.age=age;
this.eyeColor=eyecolor;
}

//person is prototype now
var myFather= new Person("john","Doe",60,"black");

//to add the property to the prototype

person.prototype.nationality="English";
person.prototype.mae=function(){
return this.fn;
}

//pass by value- pass by reference
passby value for premitive
pass by value applicable to object

//comparision operator
//DOM -Object Methods and Properties
document.getElementByID();
//Tag Name---document.getElementsByTagName('p');

//class name---document.getElementByClassName('');
//css selector--document.querySelectorALL('');


//HTML object collections
document.forms["formID"]

