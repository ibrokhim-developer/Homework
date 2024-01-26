
## Array.length.

Xususiyat `length`massivning uzunligini (o'lchamini) qaytaradi:

const fruits = ["Banana", "Orange", "Apple", "Mango"];
let size = fruits.length;

## JavaScript array toString()

JavaScript usuli `toString()`massivni (vergul bilan ajratilgan) massiv qiymatlari qatoriga aylantiradi.

const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.toString();

## JavasCript massiviga qo'shilish()

Usul `join()`, shuningdek, barcha massiv elementlarini satrga birlashtiradi.

U xuddi shunday ishlaydi `toString()`, lekin qo'shimcha ravishda siz ajratuvchini belgilashingiz mumkin:

const fruits = ["Banana", "Orange", "Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");

## JavaScript massivi pop()

Usul `pop()`massivdan oxirgi elementni olib tashlaydi:

const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();

Usul `pop()`"chiqib chiqarilgan" qiymatni qaytaradi:

const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruit = fruits.pop();

## JavaScript Array push()

Usul `push()`yangi massiv uzunligini qaytaradi:

const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.push("Kiwi");

## JavaScript massivini siljitish()

Usul `shift()`massivning birinchi elementini olib tashlaydi va qolgan barcha elementlarni pastki indeksga "o'tkazadi".

const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();

## JavaScript massivini unshift()

Usul `unshift()`massivga yangi element qo'shadi (boshida) va eski elementlarni "o'chiradi":

## JavaScript string uzunligi.

Xususiyat `length`satr uzunligini qaytaradi:

let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = text.length;

## JavaScript String charAt()

Usul `charAt()`satrdagi belgilangan indeks (pozitsiya)dagi belgini qaytaradi:

let text = "HELLO WORLD";
let char = text.charAt(0);

## JavaScript String charCodeAt()

Usul `charCodeAt()`satrdagi belgilangan indeksdagi belgi kodini qaytaradi:

Usul UTF-16 kodini qaytaradi (0 dan 65535 gacha bo'lgan butun son).

let text = "HELLO WORLD";
let char = text.charCodeAt(0);

## JavaScript String concat()

`concat()`ikki yoki undan ortiq qatorlarni birlashtiradi:

let text1 = "Hello";
let text2 = "World";
let text3 = text1.concat(" ", text2);

## JavaScript string toLowerCase()

Satr quyidagi bilan katta harfga aylantiriladi `toUpperCase()`:

Satr quyidagi bilan kichik harfga aylantiriladi `toLowerCase()`:

let text1 = "Hello World!";       // String
let text2 = text1.toLowerCase();  // text2 is text1 converted to lower

let text1 = "Hello World!";       // String
let text2 = text1.toLowerCase();  // text2 is text1 converted to lower

## JavaScript satrini takrorlash(repeat)

Usul `repeat()`satrning bir nechta nusxalari bilan qatorni qaytaradi.

Usul `repeat()`yangi qatorni qaytaradi.

Usul `repeat()`asl satrni o'zgartirmaydi.

let text = "Hello world!";
let result = text.repeat(2);

## .replace.

Usul replace()chaqirilgan satrni o'zgartirmaydi.

Usul replace()yangi qatorni qaytaradi.

Usul faqat birinchi moslikni replace()almashtiradi

let text = "Please visit Microsoft and Microsoft!";
let newText = text.replace("Microsoft", "W3Schools");


## JavaScript String split()

Agar siz satr bilan massiv sifatida ishlamoqchi bo'lsangiz, uni massivga aylantirishingiz mumkin.

text.split(",")    // Split on commas
text.split(" ")    // Split on spaces
text.split("|")    // Split on pipe

## JavaScript Object

let person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};

const person = {
  firstName: "John",
  lastName: "Doe",
  id: 5566,
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
};

##

- Object.keys({}) -> Object keys in array format

const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
const keys = Object.keys(person);

- Object.values({}) -> Object values in array format
- Object.entries({}) -> Array of elemnt ['key', 'value']
- Object.fromEntries({}) -> Array to orginal Object
- Object.assign({//target zone},{}) -> deep copy object
- Object.freeze({}) -> Object freeze object
- Deep / Shallow copy

𝐌𝐀𝐉𝐈𝐃𝐎𝐕.𝐌.𝐎, [25/01/24 21:50]
## Pure functions.

function son(a+b){
rreturn a+b;
}

## Impure functions.

let result = 0;
function son(a,b){
result = a+b;
return result;
}

## Curriying functions.

const add = (a,b,c) => a + b +c;
const curry = (a) =>{
retrn (b) =>{
return (c) => {
return a + b + c; 
};
};
};

## Closure function.

function outerFunction(x){
function innerFuntion(y){
return x + y ;
};

const closure Example =outerFunction(10);
const result = closureExample(5);
console.log(result); 

## Generator function.

function* stepGenerator() {
yiled 1;
yield 2;
yield 3;
}

const generator = stepGenerator()

console.log(generator.next());
console.log(generator.next).value);/1
console.log(generator.next).value);/2
console.log(generator.next).value);/3
console.log(generator.next).value);/undifined.