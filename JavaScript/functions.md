# פונקציות ו-ES6 ב-JavaScript

## מהי פונקציה?
פונקציה היא קטע קוד שניתן לקרוא לו ולהפעיל אותו ממקומות שונים בקוד, כדי להימנע מחזרה ולארגן את הקוד בצורה טובה יותר.

## יצירת פונקציה בסיסית
```js
function sayHello() {
    console.log("שלום עולם!");
}

sayHello(); // קריאה לפונקציה
```

## פונקציה עם פרמטרים
```js
function greet(name) {
    console.log("שלום, " + name);
}

greet("דני");
```

## פונקציה שמחזירה ערך
```js
function add(a, b) {
    return a + b;
}

let sum = add(5, 3);
console.log(sum); // 8
```

## פונקציות חץ (Arrow Functions) – ES6
צורה מקוצרת ונוחה יותר לכתיבת פונקציות.

```js
const multiply = (a, b) => {
    return a * b;
};

console.log(multiply(4, 2)); // 8
```

### Arrow Function מקוצרת
```js
const square = x => x * x;
console.log(square(5)); // 25
```

## ברירת מחדל לפרמטרים (Default Parameters) – ES6
```js
function greet(name = "אורח") {
    console.log("שלום, " + name);
}

greet(); // שלום, אורח
```

## Destructuring – ES6
שיטה לחילוץ ערכים ממערכים או אובייקטים בקלות.

### ממערך
```js
const colors = ["אדום", "כחול", "ירוק"];
const [firstColor, secondColor] = colors;
console.log(firstColor); // אדום
```

### מאובייקט
```js
const person = {
    name: "יעל",
    age: 28
};

const { name, age } = person;
console.log(name); // יעל
```

## סיכום
פונקציות הן חלק מרכזי ב-JavaScript, והחידושים של ES6 הופכים את הקוד לקצר וקריא יותר. חשוב להבין את הצורות השונות ולהשתמש בהן לפי הצורך.
