# עבודה עם ה-DOM ב-JavaScript

## מה זה DOM?
DOM (Document Object Model) הוא הממשק שמייצג את מבנה ה-HTML של העמוד כאובייקט, ומאפשר גישה ושינויים בתוכן, במבנה ובעיצוב.

## גישה לאלמנטים

### לפי מזהה (ID)
```js
const title = document.getElementById("main-title");
console.log(title.innerText);
```

### לפי מחלקה (Class)
```js
const items = document.getElementsByClassName("list-item");
console.log(items[0].innerText);
```

### לפי תגית (Tag)
```js
const paragraphs = document.getElementsByTagName("p");
console.log(paragraphs[0].innerText);
```

### querySelector – בחירה גמישה
```js
const firstItem = document.querySelector(".list-item");
console.log(firstItem.innerText);
```

### querySelectorAll – רשימת אלמנטים
```js
const allItems = document.querySelectorAll(".list-item");
allItems.forEach(item => console.log(item.innerText));
```

## שינוי תוכן

### שינוי טקסט
```js
title.innerText = "כותרת חדשה";
```

### שינוי HTML פנימי
```js
title.innerHTML = "<span>כותרת מעוצבת</span>";
```

## שינוי סגנון (CSS)
```js
title.style.color = "blue";
title.style.fontSize = "24px";
```

## הוספת והסרת מחלקות
```js
title.classList.add("highlight");
title.classList.remove("highlight");
```

## יצירה והוספת אלמנטים
```js
const newItem = document.createElement("li");
newItem.innerText = "פריט חדש";
document.querySelector("ul").appendChild(newItem);
```

## מחיקת אלמנט
```js
const list = document.querySelector("ul");
list.removeChild(list.lastElementChild);
```

## סיכום
ה-DOM הוא כלי מרכזי לעבודה עם HTML ב-JavaScript. באמצעותו ניתן לגשת, לשנות, ליצור ולהסיר אלמנטים בקלות ובמהירות.
