# אירועים ב-JavaScript

## מה זה אירוע?
אירוע (Event) הוא פעולה שמתרחשת בדפדפן, כמו לחיצה על כפתור, מעבר עכבר או הקלדה במקלדת. ב-JavaScript ניתן להאזין לאירועים ולבצע קוד בתגובה.

## האזנה לאירועים

### באמצעות מאפיין HTML
```html
<button onclick="sayHello()">לחץ עליי</button>

<script>
function sayHello() {
    alert("שלום!");
}
</script>
```

### באמצעות addEventListener (מומלץ)
```html
<button id="greet-btn">ברוך הבא</button>

<script>
const button = document.getElementById("greet-btn");
button.addEventListener("click", function() {
    alert("ברוך הבא!");
});
</script>
```

## סוגי אירועים נפוצים

### אירועי עכבר
```js
button.addEventListener("mouseover", function() {
    console.log("העכבר עבר על הכפתור");
});

button.addEventListener("mouseout", function() {
    console.log("העכבר עזב את הכפתור");
});
```

### אירועי מקלדת
```html
<input type="text" id="name-input" placeholder="הקלד את שמך">

<script>
const input = document.getElementById("name-input");
input.addEventListener("keyup", function(event) {
    console.log("הקלדת: " + event.target.value);
});
</script>
```

### אירוע טעינת עמוד
```js
window.addEventListener("load", function() {
    console.log("העמוד נטען בהצלחה");
});
```

## מניעת פעולה ברירת מחדל
```html
<a href="https://example.com" id="link">לחץ כאן</a>

<script>
const link = document.getElementById("link");
link.addEventListener("click", function(event) {
    event.preventDefault();
    alert("הקישור לא נפתח");
});
</script>
```

## סיכום
אירועים מאפשרים להוסיף אינטראקטיביות לאתר ולהגיב לפעולות המשתמש. השימוש ב-`addEventListener` הוא הדרך המומלצת לנהל אירועים בצורה גמישה ונקייה.
