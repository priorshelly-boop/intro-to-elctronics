# תמלול: AH-תרגול 1
מקור: `raw/recitations/AH-תרגול 1.pdf` (15 שקפים מוקלדים, אדיר חזן). תמלול נאמן מקריאה חזותית של השקפים, בלי תיקון והשלמה. `[לא קריא]` = לא נקרא. תיאורי ציורים בסוגריים מרובעים. מספור השקפים לפי מספר השקף בכותרת.

## שקף 1
מבוא להנדסת חשמל 361.1.1021. תרגול #1. תשפ"ז סמ' א' (2026/7). אדיר חזן.
נושאים: הקדמה, חזרה על מושגי יסוד באלקטרוסטטיקה. KCL, KVL.
אוניברסיטת בן-גוריון בנגב | ביה"ס להנדסת חשמל ומחשבים.

## שקף 2 - מבוא להנדסת חשמל 361.1.1021
- הרצאה: פרופ' גיא כהן | תרגול: אדיר חזן
- דרישות הקורס:
  - עבודות הגשה: הגשה של לפחות 80% מתרגילי הבית המפורסמים במהלך הסמסטר (**חובת הגשה**, בכדי לגשת לבחינה הסופית).
    - תרגילי בית יפורסמו ב-Moodle לפי ההתקדמות בחומר. לכל תרגיל בית שיעלה יינתן תאריך יעד סופי להגשה.
    - הגשת עבודות הבית תהיה דרך ה-Moodle בלבד, ע"י סריקתן כקובץ pdf ולהעלותה לאתר הקורס.
  - מעבר בחינה שמשקלה הוא 100% מהציון הסופי.
    - הבחינה הסופית (מועדי א' ו-ב') יהיו ללא חומר עזר. במקרה הצורך, יצורף חומר עזר מתאים.
- שעות קבלה: בתיאום מראש. hazanad@post.bgu.ac.il. שני: 15:00-16:00.
- דף המידע של הקורס - תשפ"ז מעודכן ופורסם ב-Moodle.

## שקף 3 - אלקטרוסטטיקה – מושגי יסוד
- **חוק קולון:** $\overline F_{21}=K\dfrac{q_1q_2}{r^2}\hat r$ (N) (מסגרת אדומה) [ציור: שני מטענים $q_1,q_2$ והווקטור $\vec r$ ביניהם]. $\overline F_{21}=-\overline F_{12}$.
  - $K$ הינו קבוע קולון: $K=\dfrac1{4\pi\varepsilon_0}\approx9\cdot10^9\left(\dfrac{\text{N m}^2}{\text{C}^2}\right)$
  - $\varepsilon_0=8.854\cdot10^{-12}\left(\dfrac{\text{F}}{\text{m}}\right)$ הפרמיטיביות החשמלית של הריק.
  - כיוון הכוח החשמלי תלוי בסימן: $\text{sgn}(q_1q_2)>0\Longrightarrow$ דחייה; $\text{sgn}(q_1q_2)<0\Longrightarrow$ משיכה.

## שקף 4 - אלקטרוסטטיקה – מושגי יסוד
- **שדה חשמלי:** השדה החשמלי שמייצר מטען $q_1$ מוגדר ככוח הפועל על יחידת מטען בוחן חיובי $q_2$.
  - $\overline F=K\dfrac{q_1q_2}{r^2}\hat r$ (N) $\Longrightarrow$ $\overline E=K\dfrac{q_1}{r^2}\hat r$ $\left(\dfrac NC=\dfrac Vm\right)$ (מסגרת אדומה)
- **חוק גאוס:** אחת מארבע משוואות מקסוול, הקושרת בין השטף החשמלי דרך משטח סגור לבין המטען הכולל הכלוא בתוכו.
  - $\varepsilon_0\oiint_{S_v}\overline E\cdot d\overline S=Q_{in}$ (מסגרת אדומה)
- \* יעיל לחישוב השדה החשמלי בקלות במקרים בעלי סימטריה גבוהה (למשל סימטריה כדורית, גלילית או מישורית).

## שקף 5 - תרגיל - שדה חשמלי של תייל אינסופי
חשבו את השדה החשמלי $\vec E$ הנוצר ע"י תייל אינסופי הממוקם לאורך ציר $z$, בעל צפיפות מטען קווית אחידה $\lambda$, בנקודה הנמצאת במרחק ניצב $\rho$ מהתייל. א. באמצעות חוק קולון. ב. באמצעות חוק גאוס. [ציור: תייל לאורך ציר $z$]

## שקף 6 - תרגיל - שדה חשמלי של תייל אינסופי
- א. באמצעות חוק קולון: $\overline F=K\dfrac{q_1q_2}{r_{21}^2}\hat r_{21}$ (N) $\Rightarrow$ $\overline E=\dfrac{\overline F_{21}}{q_2}=K\dfrac{q_1}{r_{21}^2}\hat r_{21}$ $\Rightarrow$ $d\overline E=K\dfrac{dq}{|\bar r-\bar r'|^3}(\bar r-\bar r')$
- $\bar r=x\hat x+y\hat y+z\hat z\longrightarrow\bar r=\rho\hat\rho+z\hat z$; $\bar r'=z'\hat z$
- (מסגרת כחולה) $|\bar r-\bar r'|=\sqrt{\rho^2+(z-z')^2}$; $(\bar r-\bar r')=\rho\hat\rho+(z-z')\hat z$
- $x\hat x+y\hat y=\rho\cos\varphi(\cos\varphi\,\hat\rho-\sin\varphi\,\hat\varphi)+\rho\sin\varphi(\sin\varphi\,\hat\rho+\cos\varphi\,\hat\varphi)=\rho\hat\rho$
- קשרים בין מערכות קואורדינטות קרטזית וגלילית: $x=\rho\cos\varphi$, $y=\rho\sin\varphi$, $z=z$; $\hat x=\cos\varphi\,\hat\rho-\sin\varphi\,\hat\varphi$, $\hat y=\sin\varphi\,\hat\rho+\cos\varphi\,\hat\varphi$, $\hat z=\hat z$; $\rho=\sqrt{x^2+y^2}$, $\varphi=\text{tg}^{-1}\left(\frac yx\right)$, $z=z$; $\hat\rho=\cos\varphi\,\hat x+\sin\varphi\,\hat y$, $\hat\varphi=-\sin\varphi\,\hat x+\cos\varphi\,\hat y$, $\hat z=\hat z$.

## שקף 7 - תרגיל - שדה חשמלי של תייל אינסופי (א, המשך)
- $d\overline E=dE_\rho\hat\rho+dE_z\hat z$
- $d\overline E=K\dfrac{dq}{|\bar r-\bar r'|^3}\rho\hat\rho+K\dfrac{dq}{|\bar r-\bar r'|^3}(z-z')\hat z$ $\Rightarrow$ $\overline E=\int d\overline E=\hat\rho\int dE_\rho+\hat z\int dE_z$
- $dq=\lambda\,dz'$
- בצד: $|\bar r-\bar r'|=\sqrt{\rho^2+(z-z')^2}$, $(\bar r-\bar r')=\rho\hat\rho+(z-z')\hat z$

## שקף 8 - תרגיל - שדה חשמלי של תייל אינסופי (א, המשך)
- $\overline E_\rho=\hat\rho\int dE_\rho=\hat\rho\displaystyle\int_{-\infty}^{\infty}K\dfrac{\lambda\,dz'}{\left[\rho^2+(z-z')^2\right]^{\frac32}}\rho$ $\Rightarrow$ $\begin{bmatrix}u=z-z'\\du=-dz'\end{bmatrix}\Rightarrow$ $\overline E_\rho=K\lambda\rho\hat\rho\displaystyle\int_{\infty}^{-\infty}\dfrac{-du}{(\rho^2+u^2)^{\frac32}}$
- $\overline E_\rho=K\lambda\rho\hat\rho\displaystyle\int_{-\infty}^{\infty}\dfrac{du}{(\rho^2+u^2)^{\frac32}}=K\lambda\rho\hat\rho\left.\dfrac{u}{\rho^2\sqrt{\rho^2+u^2}}\right|_{-\infty}^{\infty}=\left(\dfrac{K\lambda\rho}{\rho^2}+\dfrac{K\lambda\rho}{\rho^2}\right)\hat\rho=2\dfrac{K\lambda}{\rho}\hat\rho$

## שקף 9 - תרגיל - שדה חשמלי של תייל אינסופי (א, המשך)
- $\overline E_z=\hat z\int dE_z=\hat z\displaystyle\int_{-\infty}^{\infty}K\dfrac{\lambda dz'}{[\rho^2+(z-z')^2]^{\frac32}}(z-z')$ $\Rightarrow$ $\begin{bmatrix}u=z-z'\\du=-dz'\end{bmatrix}\Rightarrow$ $\overline E_z=K\lambda\hat z\displaystyle\int_{-\infty}^{\infty}\dfrac{u\,du}{(\rho^2+u^2)^{\frac32}}=0$
- $f(-u)=f(u)\Rightarrow$ פונק' אי זוגית $\Rightarrow E_z=0$
- (מסגרת אדומה) $\overline E=E_\rho\hat\rho+E_z\hat z=2\dfrac{K\lambda}{\rho}\hat\rho$

## שקף 10 - תרגיל - שדה חשמלי של תייל אינסופי (ב)
- ב. באמצעות חוק גאוס: $\oiint_{S_v}\overline E\cdot d\overline S=\dfrac{Q_{in}}{\varepsilon_0}$; $dq=\lambda\,dz'\Rightarrow Q_{in}=\lambda h$
- $\varepsilon_02\pi\rho hE_\rho=\lambda h$
- (מסגרת אדומה) $\overline E=E_\rho\hat\rho=\dfrac{\lambda}{2\pi\varepsilon_0\rho}\hat\rho=\dfrac{2K\lambda}{\rho}\hat\rho$
- בצד: $K=\dfrac1{4\pi\varepsilon_0}\approx9\cdot10^9\left(\frac{\text{N m}^2}{\text{C}^2}\right)$

## שקף 11 - אלקטרוסטטיקה – פוטנציאל חשמלי, מתח וקיבול
השדה האלקטרוסטטי משמר, ולכן העבודה בין שתי נקודות אינה תלויה במסלול אלא רק בנקודות ההתחלה והסיום.
- **פוטנציאל חשמלי:** העבודה ליחידת מטען חיובי הנדרשת להעברת מטען בוחן מאינסוף לנק' $a$ (כאשר הפוטנציאל באינסוף מוגדר כאפס, $V(\infty)=0$). $V_a=-\displaystyle\int_\infty^a\overline E\cdot d\overline\ell$ (V)
- **מתח חשמלי:** הפרש הפוטנציאלים החשמליים בין 2 נק'. $V=V_b-V_a=-\displaystyle\int_a^b\overline E\cdot d\overline\ell$ (V)
- **קבל:** קבל לוחות מורכב משני לוחות מוליכים, הנושאים מטענים שווי גודל והפוכי סימן. קיבול: היחס בין גודל המטען על אחד הלוחות לבין גודל הפרש הפוטנציאלים בין הלוחות. $C=\dfrac qV$ (F), $(C\ge0)$

## שקף 12 - תרגיל - קיבול של קבל כדורי
נתונות שתי קליפות כדוריות מוליכות וקונצנטריות, בעלות רדיוסים $a$ ו-$b$ $(a<b)$. הנושאות מטענים שווי גודל והפוכי סימן. מצאו את קיבול המערכת. $C=\dfrac qV$ (F). [ציור: שתי קליפות קונצנטריות]

## שקף 13 - תרגיל - קיבול של קבל כדורי (המשך)
- נניח כי על הקליפה הפנימית ישנו מטען $-q$, בחר משטח גאוסיאני כדורי ברדיוס $a<r<b$, מסיטריה כדורית, השדה רדיאלי ותלוי רק במרחק $r$.
- $Q_{in}=\varepsilon_0\oiint\overline E\cdot d\bar s$; $-q=\varepsilon_0\oiint\overline E\cdot d\bar s\Rightarrow-q=\varepsilon_0\oiint E_r(r)\hat r\cdot ds\,\hat r$
- $-q=\varepsilon_0E_r(r)\oiint ds=\varepsilon_04\pi r^2E(r)$ (מסגרת אדומה) $\Rightarrow\overline E(r)=-\dfrac{q}{\varepsilon_04\pi r^2}\hat r$, $a<r<b$

## שקף 14 - תרגיל - קיבול של קבל כדורי (המשך)
- $V=V_b-V_a=-\displaystyle\int_a^b\overline E\cdot d\bar\ell$; $\overline E(r)=-\dfrac{q}{\varepsilon_04\pi r^2}\hat r$
- $V=-\displaystyle\int_a^b\overline E\cdot d\bar\ell=-\int_a^b-\dfrac{q}{4\pi r^2\varepsilon_0}\hat r\cdot dr\,\hat r=\dfrac q{4\pi\varepsilon_0}\int_a^b\dfrac1{r^2}dr=\dfrac q{4\pi\varepsilon_0}\left.\dfrac1{-r}\right|_a^b=\dfrac q{4\pi\varepsilon_0}\left(\dfrac1a-\dfrac1b\right)$, $a<b$
- (מסגרת כחולה) $C=\dfrac qV=4\pi\varepsilon_0\left(\dfrac1a-\dfrac1b\right)^{-1}$

## שקף 15 - זרם חשמלי וכיווני ייחוס
- **זרם חשמלי:** $i(t)=\dfrac{dq(t)}{dt}$ (A) [ציורים: מקור מתח $v_s(t)$ עם $i_s(t)$; רכיב עם $i(t)$ ו-$+v(t)-$]
- **כיווני ייחוס במעגל חשמלי:** זרם ברכיב ינוע מ-'+' (פוט' גבוה) ל-'−' (פוט' נמוך) - בכל ענף ובכל רכיב מקובץ (לא מקור - במקור מתח זה הפוך).
- **בקורס זה**, נעסוק במעגלים **מקובצים**, בהם **חוקי קירכהוף מתקיימים**.
- **במעגלים מקובצים** – מניחים שההשפעות החשמליות מתרחשות באופן מיידי בכל נקודה במערכת (זמן מעבר האות החשמלי במעגל הוא אפסי).

## דברים לבדיקה
- בשקף 13 המשפט "מסיטריה כדורית" נקרא כפי שנראה בשקף (כנראה "מסימטריה"); נרשם ללא תיקון.
- בשקף 12 המשפט "הנושאות" נקרא כפי שנראה.
- שקף הכותרת מציין KCL, KVL כנושא, אך הקובץ מסתיים בשקף 15 בהקדמה לזרם וכיווני ייחוס.
