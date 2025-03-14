# תנאים ולולאות ב-JavaScript

## תנאים (Conditions)
תנאים מאפשרים להפעיל קוד מסוים רק אם מתקיימת בדיקה לוגית.

### if / else
```js
let age = 18;
if (age >= 18) {
    console.log("אתה יכול להצביע");
} else {
    console.log("אתה צעיר מדי להצבעה");
}
```

### else if
```js
let score = 85;
if (score >= 90) {
    console.log("ציון מצוין");
} else if (score >= 75) {
    console.log("ציון טוב");
} else {
    console.log("צריך להשתפר");
}
```

### תנאי מקוצר (Ternary Operator)
```js
let isMember = true;
let price = isMember ? 100 : 150;
console.log(price); // 100
```

## לולאות (Loops)
לולאות מאפשרות לחזור על קטע קוד מספר פעמים לפי תנאי מסוים.

### לולאת for
```js
for (let i = 0; i < 5; i++) {
    console.log("חזרה מספר: " + i);
}
```

### לולאת while
```js
let count = 0;
while (count < 3) {
    console.log("ספירה: " + count);
    count++;
}
```

### לולאת do-while
```js
let number = 0;
do {
    console.log("מספר: " + number);
    number++;
} while (number < 3);
```

### מעבר על מערכים עם forEach
```js
let colors = ["אדום", "כחול", "ירוק"];
colors.forEach(function(color) {
    console.log(color);
});
```

## סיכום
תנאים ולולאות הם כלים קריטיים לשליטה בזרימת הקוד. השימוש הנכון בהם מאפשר בניית קוד דינמי ויעיל.

