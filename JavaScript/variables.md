# משתנים, טיפוסים ואופרטורים ב-JavaScript

## מהו משתנה?
משתנה הוא מקום בזיכרון ששומר מידע שניתן לשנות ולהשתמש בו במהלך ריצת התוכנית.

## הצהרת משתנים
ב-JavaScript יש שלוש דרכים להכריז על משתנים:

### var (ישנה, פחות מומלצת)
```js
var age = 25;
console.log(age);
```

### let (מודרנית, מומלצת כאשר הערך משתנה)
```js
let name = "דני";
name = "יעל";
console.log(name);
```

### const (ערך קבוע שאינו משתנה)
```js
const PI = 3.14;
console.log(PI);
```

## סוגי נתונים (Data Types)

### מספרים (Number)
```js
let number = 10;
console.log(typeof number); // "number"
```

### מחרוזות (String)
```js
let greeting = "שלום עולם";
console.log(typeof greeting); // "string"
```

### בוליאני (Boolean)
```js
let isOnline = true;
console.log(typeof isOnline); // "boolean"
```

### מערכים (Array)
```js
let colors = ["אדום", "כחול", "ירוק"];
console.log(colors[0]); // "אדום"
```

### אובייקטים (Object)
```js
let person = {
    name: "אור",
    age: 30
};
console.log(person.name); // "אור"
```

## אופרטורים נפוצים

### אופרטורי השמה
```js
let x = 5;
x += 3; // x = x + 3
console.log(x); // 8
```

### אופרטורי השוואה
```js
console.log(5 == "5"); // true (השוואה רופפת)
console.log(5 === "5"); // false (השוואה מוחלטת)
console.log(5 !== 3); // true
```

### אופרטורי לוגיקה
```js
console.log(true && false); // false
console.log(true || false); // true
console.log(!true); // false
```

## סיכום
משתנים הם הבסיס של כל תוכנית ב-JavaScript. השימוש הנכון בהם ובטיפוסי הנתונים השונים חשוב להבנת השפה ובניית קוד נקי ויעיל.

