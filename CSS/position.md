# מיקום CSS
<div dir="rtl">
מיקום CSS הוא מושג יסודי המאפשר לך לשלוט בפריסת האלמנטים בדף האינטרנט שלך. הוא קובע כיצד אלמנטים ממוקמים ומתקשרים עם אלמנטים אחרים בזרימת המסמך. התכונה `position` משמשת לציון סוג שיטת המיקום עבור אלמנט.

### ערכים נפוצים עבור `position`

<ul dir="rtl">
<li>**`static`**</li>
<li>**`relative`**</li>
<li>**`absolute`**</li>
<li>**`fixed`**</li>
<li>**`sticky`**</li>
</ul>

### השוואה והסבר

<div dir="rtl">
  <h3 dir="rtl"><strong>`static`</strong></h3>
  <ul dir="rtl">
    <li dir="rtl">ערך ברירת המחדל. אלמנטים ממוקמים בהתאם לזרימת המסמך הרגילה.</li>
    <li dir="rtl">התכונות `top`, `right`, `bottom`, `left`, ו-`z-index` אינן משפיעות.</li>
  </ul>
</div>

### דוגמה:
```css
.static {
  position: static;
}
```

<div dir="rtl">
  <h3 dir="rtl"><strong>`relative`</strong></h3>
  <ul dir="rtl">
    <li dir="rtl">ממוקם יחסית למיקום הרגיל שלו בזרימת המסמך.</li>
    <li dir="rtl">ניתן להשתמש ב-`top`, `right`, `bottom`, ו-`left` כדי להזיז את האלמנט ממיקומו המקורי.</li>
    <li dir="rtl">תוכן אחר לא יתאים עצמו כדי להתאים לרווח שנשאר על ידי האלמנט.</li>
  </ul>
</div>

### דוגמה:
```css
.relative {
  position: relative;
  top: 20px;
  left: 20px;
}
```

<div dir="rtl">
  <h3 dir="rtl"><strong>`absolute`</strong></h3>
  <ul dir="rtl">
    <li dir="rtl">מוסר מזרימת המסמך הרגילה. לא נוצר מרווח עבור האלמנט בפריסת הדף.</li>
    <li dir="rtl">ממוקם יחסית לאב הממוקם הקרוב ביותר (שאינו `static`). אם לא קיים אב כזה, הוא ממוקם יחסית לבלוק המכיל הראשוני (בדרך כלל החלון).</li>
    <li dir="rtl">התכונות `top`, `right`, `bottom`, ו-`left` קובעות את המיקום הסופי.</li>
  </ul>
</div>

### דוגמה:  
```css
.absolute {
  position: absolute;
  top: 30px;
  right: 10px;
}
```

<div dir="rtl">
  <h3 dir="rtl"><strong>`fixed`</strong></h3>
  <ul dir="rtl">
    <li dir="rtl">מוסר מזרימת המסמך הרגילה. המסמך ואלמנטים אחרים מתנהגים כאילו הוא כלל לא קיים.</li>
    <li dir="rtl">ממוקם יחסית לחלון, מה שאומר שהוא תמיד נשאר באותו מקום גם אם הדף גולל.</li>
    <li dir="rtl">שימושי ליצירת סרגל ניווט שנשאר בראש המסך בזמן גלילה למטה.</li>
  </ul>
  </div>

### דוגמה:  
```css
.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
}
```
<div dir="rtl">
  <h3 dir="rtl"><strong>`sticky`</strong></h3>
  <ul dir="rtl">
    <li dir="rtl">היברידי של מיקום יחסי וקבוע. האלמנט מטופל כ-`relative` עד שהוא חוצה נקודה מסוימת, ואז הוא מטופל כ-`fixed`.</li>
    <li dir="rtl">משמש לעתים קרובות עבור כותרות שנגללות עם התוכן אך נדבקות לחלק העליון של החלון כאשר מגיעות לסף מסוים.</li>
  </ul>
</div>

### דוגמה:  
```css
.sticky {
  position: sticky;
  top: 0;
}
```


### מקרי שימוש מעשיים

<ul dir="rtl">
<li dir="rtl"><strong>`static`</strong>: לא מצוין לעתים קרובות, מכיוון שזה ברירת המחדל. השתמש בו כדי לאפס כל מיקום שהוחל קודם לכן.</li>
<li dir="rtl"><strong>`relative`</strong>: שימושי להתאמת מיקום אלמנט מבלי להשפיע על פריסת המסמך. מעולה לדחיפה קלה של אלמנטים.</li>
<li dir="rtl"><strong>`absolute`</strong>: מושלם ליצירת תפריטים נפתחים או חלונות מודאליים שצפים מעל תוכן אחר.</li>
<li dir="rtl"><strong>`fixed`</strong>: אידיאלי ליצירת אלמנטים שנשארים גלויים, כמו כותרות או כותרות תחתונות דביקות, ללא קשר לגלילה.</li>
<li dir="rtl"><strong>`sticky`</strong>: הטוב ביותר עבור אלמנטים שצריכים להיגלל עם התוכן אך להישאר קבועים בנקודה מסוימת, כמו סרגל ניווט דביק.</li>
</ul>
הבנת הקשרי מיקום אלה היא קריטית לשליטה יעילה בפריסה ב-CSS, ומאפשרת עיצובים רב-תכליתיים ודינמיים.
</div>
