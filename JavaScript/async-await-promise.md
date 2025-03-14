## שימוש ב- Promise ו-Async/Await ב-JavaScript

## מה זה Promise?
האובייקט Promise הוא שמייצג פעולה אסינכרונית שיכולה להסתיים בהצלחה (resolve) או בכישלון (reject).

## יצירת Promise
```js
const fetchData = () => {
    return new Promise((resolve, reject) => {
        setTimeout(() => {
            const success = true;
            if (success) {
                resolve("הנתונים נטענו בהצלחה");
            } else {
                reject("שגיאה בטעינת הנתונים");
            }
        }, 2000);
    });
};
```

## שימוש ב-Promise עם then ו-catch
```js
fetchData()
    .then(data => {
        console.log(data);
    })
    .catch(error => {
        console.error(error);
    });
```

## מה זה Async/Await ?
תחביר נוח וקריא יותר לעבודה עם פעולות אסינכרוניות.

## פונקציה אסינכרונית
```js
const loadData = async () => {
    try {
        const data = await fetchData();
        console.log(data);
    } catch (error) {
        console.error(error);
    }
};

loadData();
```

## Fetch API – קריאת נתונים משרת
```js
const getUser = async () => {
    try {
        const response = await fetch("https://jsonplaceholder.typicode.com/users/1");
        const user = await response.json();
        console.log(user);
    } catch (error) {
        console.error("שגיאה בשליפת הנתונים", error);
    }
};

getUser();
```

## סיכום
לסיכום, Promise ו-Async/Await הם כלים חזקים לעבודה עם קוד אסינכרוני ב-JavaScript. השימוש ב-`await` הופך את הקוד לקריא וברור יותר בהשוואה ל-`then` ו-`catch`.
