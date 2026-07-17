<div dir="rtl" align="right">

# 📘 מדריך Git ו-GitHub

מדריך מהיר וברור לעבודה עם Git ו-GitHub — יצירת ריפו, הורדה, העלאת שינויים ומעבר בין גרסאות.

> 💡 לכל בלוק פקודות יש כפתור העתקה (📋) שמופיע בפינה כשמעבירים עליו את העכבר.

---

## 🆕 יצירת ריפו חדש בגיטהאב וקישורו לתיקיה במחשב

**1.** נכנסים ל־ <code dir="ltr">https://github.com</code>, מתחברים לחשבון, נכנסים ל־ **Repositories** ולוחצים על הכפתור הירוק **New**

או פשוט: [https://github.com/new](https://github.com/new)

**2.** כותבים את שם הריפו ב־ **Repository name**, גוללים לתחתית ולוחצים על הכפתור הירוק **Create repository**

**3.** נכנסים לתוך התיקיה במחשב שרוצים לקשר, כותבים למעלה `CMD` ולוחצים על **Enter**

**4.** מריצים את הפקודות הבאות:

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/gefNschlisL/my_repo.git
git push -u origin main
```

| פקודה | הסבר |
|---|---|
| `git add .` | הקובץ או הקבצים שרוצים להעלות. נקודה מעלה את כולם |
| `git commit -m "ההערה של הקומיט"` | ההערה של הקומיט |
| `git remote add origin ...שם_הריפו.git` | שם הריפו |

---

## ⬇️ הורדת ריפו קיים מגיטהאב לתיקיה שתיווצר ותקושר אליו

**1.** נכנסים ל־ <code dir="ltr">https://github.com/[שם המשתמש בגיטהאב]</code> (לדוגמה [https://github.com/gefNschlisL](https://github.com/gefNschlisL)) ‏› **Repositories** ובוחרים בריפו שרוצים,

או פשוט: <code dir="ltr">https://github.com/[שם המשתמש בגיטהאב]/שם_הריפו</code>

**2.** לוחצים על הכפתור הירוק **Code** ומעתיקים את הקישור

**3.** נכנסים לתוך התיקיה במחשב שאליה רוצים להוריד, כותבים למעלה `CMD` ולוחצים על **Enter**

**4.** כותבים `git clone` + רווח + מדביקים את הקישור ולוחצים על **Enter**

```bash
git clone https://github.com/gefNschlisL/שם_הריפו.git
```

---

## 🔼 העלאת קבצים שהשתנו לגיטהאב מתיקיה שכבר מקושרת

**1.** נכנסים לתוך התיקיה המקושרת במחשב, כותבים למעלה `CMD` ולוחצים על **Enter**

**2.** מריצים את הפקודות הבאות:

```bash
git add .
git commit -m "first commit"
git push
```

| פקודה | הסבר |
|---|---|
| `git add .` | הקובץ או הקבצים שרוצים להעלות. נקודה מעלה את כולם |
| `git commit -m "first commit"` | ההערה של הקומיט |

---

## 🔽 הורדת קומיטים חדשים מגיטהאב לתיקיה שכבר מקושרת

**1.** נכנסים לתוך התיקיה המקושרת במחשב, כותבים למעלה `CMD` ולוחצים על **Enter**

**2.** כותבים ולוחצים על **Enter**:

```bash
git pull origin main
```

---

## 🕹️ מעבר בין גרסאות שנמצאות בתיקיה של המחשב

**1.** נכנסים ל־ <code dir="ltr">https://github.com/[שם המשתמש בגיטהאב]</code> (לדוגמה [https://github.com/gefNschlisL](https://github.com/gefNschlisL)) ‏› **Repositories** ובוחרים בריפו שרוצים,

או פשוט: <code dir="ltr">https://github.com/[שם המשתמש בגיטהאב]/שם_הריפו</code>

**2.** לוחצים על **Commits** שמתחת לכפתור הירוק, ומעתיקים את ההאש (hash) של הקומיט שאליו רוצים לעבור

**3.** נכנסים לתוך התיקיה המקושרת במחשב, כותבים למעלה `CMD` ולוחצים על **Enter**

**4.** כותבים `git checkout` + רווח + מדביקים את ההאש ולוחצים על **Enter**

```bash
git checkout <commit-hash>
```

</div>
