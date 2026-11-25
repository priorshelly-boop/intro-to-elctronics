# תמלול: AH-תרגול 3
מקור: `raw/recitations/AH-תרגול 3.pdf` (44 שקפים מוקלדים, אדיר חזן). תמלול נאמן מקריאה חזותית של השקפים, בלי תיקון והשלמה. `[לא קריא]` = לא נקרא. תיאורי ציורים בסוגריים מרובעים. מספור לפי מספר השקף בכותרת.

## שקף 1
מבוא להנדסת חשמל 361.1.1021. תרגול #3. תשפ"ז סמ' א' (2026/7). אדיר חזן.
נושאים: המשך שקילויות במעגלים חשמליים: התמרת מקורות - שקול תבנין/נורטון. הדיודה כנגד - מעגל קטימה. פונק' נוספות - צורות גל ופונ' הלם.

## שקף 2 - תזכורת: נגדים Resistors
נגד הינו רכיב בעל שני הדקים שבו מתקיים **בכל רגע** קשר בין המתח הנופל עליו לבין הזרם העובר דרכו: $v(t)=f(i(t),t)$. העקומה המתארת את הקשר $v$–$i$ **בכל רגע** נקראת אופיין הנגד. [ציור: נגד עם $i_R$, $+v_R-$]
| תכונות | לינארי (L) | לא לינארי (NL) |
|---|---|---|
| קבוע בזמן (TI) | $v(t)=Ri(t)$ [גרף: קו ישר דרך הראשית] | $v(t)=f(i(t))$ |
| משתנה בזמן (TV) | $v(t)=R(t)i(t)$ | $v(t)=f(i(t),t)$ |
| נגד LTI פאסיבי אם ורק אם: $R\ge0$ | $G\equiv\frac1R$, $[G]=\Omega^{-1}=\mho$ | אופיין הנגד $f_R$ $\Leftarrow$ הקשר $v_R$–$i_R$ |
| חיבור $N$ נגדים בטור | $R_{eq}=\sum_{k=1}^NR_k$, $G_{eq}=\left(\sum_{k=1}^N\frac1{G_k}\right)^{-1}$ | $i_{eq}=i_k$, $v_{eq}=\sum_{k=1}^Nv_k$ |
| חיבור $N$ נגדים במקביל | $R_{eq}=\left(\sum_{k=1}^N\frac1{R_k}\right)^{-1}$, $G_{eq}=\sum_{k=1}^NG_k$ | $v_{eq}=v_k$, $i_{eq}=\sum_{k=1}^Ni_k$ |

## שקף 3 - תזכורת: מחלק זרם/מתח Current/Voltage Division
- עבור חיבור שני נגדים **לינארים** בטור: $v_{R_1}=v_{in}\dfrac{R_1}{R_1+R_2}$, $v_{R_2}=v_{in}\dfrac{R_2}{R_1+R_2}$. עבור חיבור $N$ נגדים **לינארים** בטור: $v_{R_i}=v_{in}\dfrac{R_i}{\sum_{k=1}^NR_k}$
- עבור חיבור שני נגדים **לינארים** במקביל: $i_{R_1}=i_{in}\dfrac{R_2}{R_1+R_2}$, $i_{R_2}=i_{in}\dfrac{R_1}{R_1+R_2}$. עבור חיבור $N$ נגדים **לינארים** במקביל: $i_{R_i}=i_{in}\dfrac{R_{tot}}{R_i}$, $R_{tot}=\left(\sum_{k=1}^N\frac1{R_k}\right)^{-1}$

## שקף 4 - תזכורת: מקורות ב"ת Independent Sources
מקורות ב"ת כופים מתח / זרם נתון, ללא תלות במתחים או בזרמים אחרים במעגל.
- **מקור מתח:** [סמל $V_0,v_s(t)$ עם $v^+,v^-$, $i_s(t)$; גרף $v(t)$ מול $i(t)$: קו אופקי ב-$V_0$; $v_s:=v^+-v^-$; הארקה]
- **מקור זרם:** [סמל $I_0,i_s(t)$; גרף: קו אנכי ב-$I_0$]
- $R\to\infty$: $OC:i=0$. $R=0$: $SC:v=0$.

## שקף 5 - שקול תבנין ונורטון Thévenin & Norton Equivalent Circuits
התמרת מקורות Source Transformation.
- Thévenin: מקור $v_{Th}$ בטור עם $R_{eq}$ ועומס $R_L$; $v=v_{Th}\dfrac{R_L}{R_L+R_{eq}}$
- Norton: מקור $i_N$ במקביל ל-$R_{eq}$ ועומס $R_L$; $v=iR_L=i_N\dfrac{R_{eq}}{R_L+R_{eq}}R_L$
- שקילות: $R_{eq}=R_{Th}=R_N$; $v_{Th}\dfrac{R_L}{R_L+R_{eq}}=i_N\dfrac{R_{eq}}{R_L+R_{eq}}R_L$; (מסגרת אדומה) $v_{Th}=R_{eq}\,i_N$
- שני המעגלים שקולים מבחינת העומס. עבור כל עומס שנחבר להדקים, נקבל את אותו מתח ואת אותו זרם.

## שקף 6 - תרגיל - התמרת מקורות
עבור המעגל הבא, [מעגל: מקור זרם 4 A משמאל; $5\ \Omega$ במקביל; $4\ \Omega$ ו-$1\ \Omega$ בטור בענף העליון, עם מקור זרם 10 A במקביל ל-$1\ \Omega$; $40\ \Omega$ בטור עם מקור מתח 10 V בענף אנכי; $2\ \Omega$ בענף הימני; $I_0$ בענף העליון]. מצאו את $I_0$.

## שקף 7 - תרגיל - התמרת מקורות (פתרון)
- $v_{Th}=R_{eq}\,i_N$; $R_{eq}=R_{Th}=R_N$
- $v_{Th}=1\cdot10=10$ (V) (מקור 10 A במקביל ל-$1\ \Omega$ הופך למקור 10 V בטור עם $1\ \Omega$); $v_{Th}=5\cdot4=20$ (V) (מקור 4 A במקביל ל-$5\ \Omega$ הופך למקור 20 V בטור עם $5\ \Omega$)
- [מעגל אחרי ההמרה: $5\ \Omega$ ו-20 V משמאל; $4\ \Omega$, $1\ \Omega$ ו-10 V בטור למעלה; $40\ \Omega$ ו-10 V; $2\ \Omega$; $I_0$]

## שקף 8 - תרגיל - התמרת מקורות (המשך)
- שני מקורות מתח בטור: $V_1-V_2$ [ציור: שני מקורות בטור $\Rightarrow$ מקור אחד $V_1-V_2$ (מסגרת מקווקווה אדומה)]
- $V_{eq}=20-10=10$ (V); $R_{eq}=5+4+1=10$ ($\Omega$)
- [מעגל: $10\ \Omega$ ו-10 V משמאל, $40\ \Omega$ ו-10 V, $2\ \Omega$, $I_0$]

## שקף 9 - תרגיל - התמרת מקורות (המשך)
- $\dfrac{v_{Th}}{R_{eq}}=i_N$; $R_{eq}=R_{Th}=R_N$
- $I_{N1}=\dfrac{10}{10}=1$ (A); $I_{N2}=\dfrac{10}{40}=0.25$ (A)
- [מעגל: מקור זרם 1 A עם $10\ \Omega$ במקביל; מקור זרם 0.25 A עם $40\ \Omega$ במקביל; $2\ \Omega$; $I_0$]

## שקף 10 - תרגיל - התמרת מקורות (המשך)
- [שני מקורות זרם במקביל: $I_1$ ו-$I_2$ $\Rightarrow$ מקור $I_1+I_2$]
- $I_{eq}=1+0.25=1.25$ (A); $R_{eq}=10(\Omega)\parallel40(\Omega)=8$ ($\Omega$)
- [מעגל: 1.25 A, $8\ \Omega$, $2\ \Omega$, $I_0$]

## שקף 11 - תרגיל - התמרת מקורות (סיום)
- Thévenin: [מעגל: 10 V, $8\ \Omega$, עומס $2\ \Omega$, $I_0$] $I=\dfrac{V_{Th}}{R_{tot}}\Rightarrow$ (מסגרת אדומה) $I_0=\dfrac{V_{Th}}{R_{Th}+R_L}=\dfrac{10}{8+2}=1$ (A)
- $v_{Th}=R_L\ i_N$ (חצים למעגל המקורי)
- Norton: [מעגל: 1.25 A, $8\ \Omega$, עומס $2\ \Omega$] $I_{R_i}=I_{in}\dfrac{R_{tot}}{R_i}\Rightarrow$ (מסגרת אדומה) $I_0=I_{in}\dfrac{R_N}{R_N+R_L}=1.25\dfrac8{8+2}=1$ (A)

## שקף 12 - נגדים Resistors
נגד הוא רכיב בעל שני הדקים שבו מתקיים **בכל רגע** קשר בין המתח הנופל עליו לבין הזרם העובר דרכו: $v(t)=f(i(t),t)$. העקומה המתארת את הקשר $v$–$i$ **בכל רגע** נקראת אופיין הנגד.
| תכונות | לינארי (L) | לא לינארי (NL) (נקרא גם מוליך לא-אוהמי) |
|---|---|---|
| קבוע בזמן (TI) | $v(t)=Ri(t)$ | $v(t)=f(i(t))$ |
- [ציורים: $R\to\infty,G=0$: $OC:i=0$ (גרף $i$ מול $v$: קו על ציר $v$); $R=0,G\to\infty$: $SC:v=0$ (גרף: קו על ציר $i$); $G(\mho)\equiv(R(\Omega))^{-1}$]
- [דיודה $i_d$, $+v_d-$; גרף $i_d$ מול $v_d$: קצר $v_d=0,i_d\ge0$; נתק $i_d=0,v_d\le0$]

## שקף 13 - דיודה Diode
דיודה אידיאלית היא רכיב בעל 2 הדקים, לא-ליניארי וקבוע בזמן, המתואר באמצעות אופיין מתח-זרם $v(t)=f(i(t))$ **בכל רגע** $\Leftarrow$ נגד NLTI המקיים.
- **לדיודה אידיאלית 2 מצבי עבודה:** הולכה (סגורה) - קצר. קטעון (פתוחה, לא מוליכה) - נתק.
- [אופיין דיודה אידיאלית: קצר $v_d=0,i_d\ge0$; נתק $i_d=0,v_d\le0$; אופיין דיודה מעשית: $i(t)=I_s\left(e^{qv(t)/\eta kT}-1\right)$ עם $I_s$ בצד שלילי; איור: Anode (+) P, N Cathode (−)]
- Types of semiconductor diodes: Light-Emitting Diode (LED), Photodiode, Solar Cells.

## שקף 14 - תרגיל - שאלה ממבחנים
עבור המעגל הבא, $v_{in}$ הינו אות הכניסה למעגל. $E>0$ מקור מתח קבוע, אידיאלי וב"ת. $R>0$. דיודות אידיאליות $D_1,D_2$. [מעגל: $v_{in}$, $R$ בטור, $D_1$ ו-$E$ בענף אנכי; $D_2$ ו-$E$ בענף אנכי נוסף, $v_{out}$ על ההדקים]
1) מצאו את מתח המוצא $v_{out}$ לכל אות כניסה $v_{in}$.
2) מה ישתנה אם נחבר במוצא נגד לינארי?
3) איך יראה אות המוצא $v_{out}(t)$ עבור אות הכניסה $v_{in}(t)=[3\sin(2\pi ft)]$ V כאשר כל הרכיבים בעלי ערך יחידה.

## שקף 15 - תרגיל - מעגל קטימה
עבור תרגילים עם דיודות: מניחים מצבי עבודה של הדיודות. לכל דיודה יש שני מצבי עבודה (קצר / נתק) $\Leftarrow$ סה"כ 4 מצבים למעגל. מחשבים זרם / מתח של הדיודה יחד עם התנאי עבור כל מצב העבודה - ובודקים אם המצבים אפשריים (לא יוצרים סתירה). [אופיין הדיודה האידיאלית]

## שקף 16 - תרגיל - מעגל קטימה (מצב 1)
מצאו את מתח המוצא $v_{out}$ לכל אות כניסה $v_{in}$. נבדוק את כל המצבים האפשריים:
1. שתי הדיודות $D_1,D_2$ בהולכה (בקצר). [מעגל: $v_{out}=E$ $\ne$ $v_{out}=-E$, $E>0$, מסומן X]
מצב **לא אפשרי**, יוצר סתירה: מקור מתח **אידיאלי** המחובר **במקביל** גובר על כל מקור אנרגיה אחר $\Leftarrow$ **לא** ייתכן **מקורות מתח אידיאליים** שמחוברים **במקביל** שכופים מתחים שונים על אותן צמתים.

## שקף 17 - תרגיל - מעגל קטימה (מצב 1, המשך)
מצב **לא אפשרי**, מכיוון שיוצר סתירה עם KVL בחוג האמצעי: KVL @1: $-E-v_{D1}-v_{D2}-E=0$; בקצר $D_1,D_2$ $\Rightarrow v_{D1},v_{D2}=0$ $\Rightarrow$ $-E-E\ne0$. נתון: $E>0$ מקור מתח קבוע, אידיאלי וב"ת.

## שקף 18 - תרגיל - מעגל קטימה (מצב 2)
2. שתי הדיודות $D_1,D_2$ בקטעון (בנתק). [$v_{D1}<0$, $v_{D2}<0$] אין מסלול לזרם $\Rightarrow$ $i=0$, $v_R=0$. (מסגרת אדומה) $v_{out}=v_{in}$

## שקף 19 - תרגיל - מעגל קטימה (מצב 2, המשך)
- KVL @2: $-v_{in}+v_R+v_{D1}+E=0$; $i=0\Rightarrow v_R=0$; $\Rightarrow v_{D1}=v_{in}-E$. $v_{D1}<0$ בנתק $D_1$ $\Rightarrow v_{in}-E<0\Rightarrow$ (מסגרת כחולה) $v_{in}<E$
- KVL @3: $-v_{in}-v_{D2}-E=0\Rightarrow v_{D2}=-v_{in}-E$. $v_{D2}<0$ בנתק $D_2$ $\Rightarrow-v_{in}-E<0\Rightarrow$ (מסגרת כחולה) $-E<v_{in}$
- (מסגרת אדומה) $v_{out}=v_{in}$, $-E<v_{in}<E$

## שקף 20 - תרגיל - מעגל קטימה (מצב 3)
3. הדיודה $D_1$ בהולכה (בקצר), ו-$D_2$ בקטעון (בנתק). [$+v_R-$, $i_{D1}$, $v_{D2}<0$] (מסגרת אדומה) $v_{out}=E$. (אופיין הדיודה בצד: קצר $v_d=0,i_d>0$; נתק $i_d=0,v_d<0$)

## שקף 21 - תרגיל - מעגל קטימה (מצב 3, המשך)
- KVL @2: $-v_{in}+v_R+v_{D1}+E=0$; $v_{D1}=0$ בקצר $D_1$ $\Rightarrow-v_{in}+v_R+E=0\overset{R\ LTI}{\Longrightarrow}-v_{in}+Ri+E=0$ $\Rightarrow i=\dfrac{v_{in}-E}R$
- עבור מעגל טורי: KCL @$a$: $i_R=i_{D1}\triangleq i$
- $i_{D1}>0$ בקצר $D_1$ $\Rightarrow\dfrac{v_{in}-E}R>0\Rightarrow$ (מסגרת אדומה) $v_{in}>E$
- (מסגרת אדומה) $v_{out}=E$, $E<v_{in}$
- בדיקה ש-$D_2$ בקטעון: KVL @1: $-E-v_{D2}-E=0\Rightarrow v_{D2}=-2E<0$. $D_2$ אכן בקטעון (בנתק).

## שקף 22 - תרגיל - מעגל קטימה (מצב 4)
4. הדיודה $D_1$ בקטעון (בנתק), ו-$D_2$ בהולכה (בקצר). [$v_{D1}<0$, $i_{D2}$] (מסגרת אדומה) $v_{out}=-E$.

## שקף 23 - תרגיל - מעגל קטימה (מצב 4, המשך)
- KVL @3: $-v_{in}+v_R-v_{D2}-E=0$; $v_{D2}=0$ בקצר $D_2$ $\Rightarrow-v_{in}+v_R-E=0\overset{R\ LTI}{\Longrightarrow}-v_{in}+Ri-E=0\Rightarrow i=\dfrac{v_{in}+E}R$
- עבור מעגל טורי: KCL @$a$: $i_R=-i_{D2}\triangleq i$
- $i_{D2}>0$ בקצר $D_2$ $\Rightarrow-i=-\dfrac{v_{in}+E}R>0\Rightarrow$ (מסגרת אדומה) $-E>v_{in}$
- (מסגרת אדומה) $v_{out}=-E$, $v_{in}<-E$
- בדיקה ש-$D_1$ בקטעון: KVL @1: $-E-v_{D1}-E=0\Rightarrow v_{D1}=-2E<0$. $D_1$ אכן בקטעון (בנתק).

## שקף 24 - תרגיל - מעגל קטימה (סיכום)
1) מצאו את מתח המוצא $v_{out}$ לכל אות כניסה $v_{in}$. $v_{out}=\begin{cases}E,&E<v_{in}\\v_{in},&-E\le v_{in}\le E\\-E,&v_{in}<-E\end{cases}$ [גרף $v_{out}$ מול $v_{in}$: קו אופקי ב-$E$, ישר בשיפוע 1 בין $-E$ ל-$E$, אופקי ב-$-E$]
2) מהו מתח המוצא $v_{out}$ לכל אות כניסה $v_{in}$ כאשר מחוברים במקביל למוצא נגד לינארי $R_L$? (ללא פתרון בשקף)

## שקף 25 - תרגיל - מעגל קטימה (3)
3) איך יראה אות המוצא $v_{out}(t)$ עבור אות הכניסה $v_{in}==[3\sin(2\pi ft)]$ V כאשר כל הרכיבים בעלי ערך יחידה. $v_{out}=\begin{cases}E,&E<v_{in}\\v_{in},&-E\le v_{in}\le E\\-E,&v_{in}<-E\end{cases}$; $v_{in}(t)=3\sin(2\pi ft)$. [גרף: $v_{in}(t)$ (כחול מקווקו, סינוס) ו-$v_{out}(t)$ (אדום, סינוס קטום ב-$\pm E$)]

## שקף 26 - Typical Waveforms - צורות גל נפוצות
- **The Constant - קבוע:** $f(t)=K$, $\forall t$, $K=const$. [גרף: קו אופקי ב-$K$] [סמלים: מקור זרם $I_0$; מקור מתח $V_0$ עם $I_0$] זרם ישר (DC) Direct Current
- **The Sinusoid - סינוסואידה:** $f(t)=A\cos(\omega t+\phi)$. [גרף: סינוס, $T=2\pi/\omega$, אמפליטודה $A$, הסטה $\left[\frac\phi\omega\right]=\text{sec}$]
  - $A\ge0$ - אמפליטודה (משרעת התנודות).
  - $\omega$ - תדירות זוויתית: $\omega=2\pi f=2\pi/T$, $[f]=\text{Hz}$, $[\omega]=\text{rad/sec}$.
  - $\phi$ - פאזה (זווית המופע), $[\phi]=\text{rad}$ (ניתן לייצוג גם ב-°).
  - זרם חילופין (AC) Alternating Current [סמלים: מקור זרם $i_s(t)$; מקור מתח סינוסי $v_s(t)$ עם $i_s(t)$]

## שקף 27 - Typical Waveforms
- **The Unit Step - מדרגת יחידה:** $u(t)=\begin{cases}0,&t<0\\1,&0<t\end{cases}$ [גרף]. פונ' בעלת אי-רציפות מהסוג הראשון בנק' $t=0$. $\lim_{t\to0^-}u(t)\neq\lim_{t\to0^+}u(t)$. [מעגל: סוללה $V_0=1$ V ומתג ב-$t=0$ $\to$ מקור מתח $v_s(t)=u(t)$]
- **The Unit Ramp - שיפוע (רמפה) יחידה:** $r(t)=\begin{cases}0,&t<0\\t,&0\le t\end{cases}$; $r(t)=t\,u(t)$, $\forall t$. [גרף]
  - ניתן לקשר את פונ' השיפוע למדרגה יחידה: פונ' רציפה, $r(0)\triangleq0$. הנגזרת הראשונה אינה קיימת באופן הקלאסי בנק' $t=0$ (הנגזרות החד-צדדיות שונות). הפונ' הקדומה של $r(t)$ גם רציפה: $\int_{-\infty}^tr(t')dt'=\dfrac{t^2}2u(t)$
  - (מסגרת אדומה) $\int_{-\infty}^tu(t')dt'=r(t)\iff\dfrac{dr(t)}{dt}=u(t)$

## שקף 28 - Typical Waveforms
איך תראה צורת הגל $-u(t_0-t)$ כפונ' של הזמן?
- **הזזה בזמן:** $u(t-t_0)=\begin{cases}0,&t<t_0\\1,&t>t_0\end{cases}$ [גרף]
- **היפוך בזמן:** $u(-t)=\begin{cases}1,&t<0\\0,&t>0\end{cases}$ [גרף]
- **הזזה + היפוך בזמן + שיקוף:** $-u(t_0-t)=\begin{cases}-1,&t<t_0\\0,&t>t_0\end{cases}$ [גרף]

## שקף 29 - Typical Waveforms
בעזרת מניפולציות שונות של הפונ' הבסיסיות ניתן לתאר (וליצור) פונ' נוספות. למשל, דופק (פולס) מלבני Rectangular Pulse:
- $\Pi\left(\dfrac t{2a}\right)=\text{rect}\left(\dfrac t{2a}\right)$ [גרף: מלבן בגובה 1 בין $-a$ ל-$a$] $=u(t+a)-u(t-a)$ [גרפים של שתי מדרגות]
- הזזה + שיקוף יחסית לציר הזמן: $\text{rect}\left(\frac t{2a}\right)=u(t+a)-u(t-a)$
- הזזה · הזזה והיפוך בזמן: $\text{rect}\left(\frac t{2a}\right)=u(t+a)\,u(a-t)$
- $a>0$

## שקף 30 - Typical Waveforms - The Unit Pulse - דופק (פולס) יחידה
- שינוי קנה מידה של פונ' המלבן, **תמיד עם שטח 1**: $\int_{-\infty}^\infty P_\Delta(t)dt=1$, $\forall\Delta>0$
- גם את פונ' פולס היחידה $P_\Delta(t)$ ניתן לתאר בעזרת פונ' מדרגה: $P_\Delta(t)=\frac1\Delta[u(t)-u(t-\Delta)]$, $\forall t$; $P_\Delta(t)=\frac1\Delta u(t)\,u(\Delta-t)$, $\forall t$
- $P_\Delta(t)=\begin{cases}0,&t<0\\\frac1\Delta,&0<t<\Delta\\0,&\Delta<t\end{cases}$, $\Delta>0$. [גרף: מלבן בגובה $1/\Delta$ מ-0 עד $\Delta$]

## שקף 31 - Typical Waveforms - The Unit Impulse - מתקף יחידה
פונ' מוכללת דלתא / פונ' דיראק (Dirac) / פונ' הלם.
- הגדרות שקולות:
  - נאמר כי הגבול החלש של משפחת הפונ' החד פרמטרית $P_\Delta(t)$: $\delta(t)=W_-\lim_{\Delta\to0}P_\Delta$. אם לכל פונ' $f(t)$ אינטגרבילית בסביבת אפס ורציפה באפס, מתקיים: $\int_{-\infty}^\infty\delta(t)f(t)dt=\lim_{\Delta\to0}\int_{-\infty}^\infty P_\Delta(t)f(t)dt=f(0)$
  - $\delta(t)=0,\ \forall t\ne0\ \Rightarrow\begin{cases}0,&t\ne0\\singular,&t=0\end{cases}$. הסינגולריות סביב האפס היא כזו שעבור $\forall\xi>0$ (קטן כרצוננו) מתקיים: $\int_{-\xi}^\xi\delta(t')dt'=1$. כלומר לפונ' $\delta(t)$ יש גודל מוגדר היטב בתוך האינטגרל המוכלל.
- [גרף: $\delta(t)$ Symbol !!: חץ בגובה 1 ב-0]

## שקף 32 - Typical Waveforms
- פונקציה מוכללת דלתא $\delta(t)$ [$P_\Delta(t)$, $\Delta\to0$; גרפים]
- (מסגרת אדומה) $\lim_{\Delta\to0}P_\Delta(t)=\begin{cases}0,&t\ne0\\singular,&t=0\end{cases}$; $\int_{-\infty}^\infty P_\Delta(t')dt'=1,\ \forall\Delta>0\Longrightarrow$ (מסגרת אדומה) $\lim_{\Delta\to0}\int_{-\infty}^\infty P_\Delta(t')dt'=1$ $>$ $\int_{-\infty}^\infty\lim_{\Delta\to0}P_\Delta(t')dt'=0$
- $\Downarrow$ $\lim_{\Delta\to0}\int(\cdot)\not\Rightarrow\int\lim_{\Delta\to0}(\cdot)$; $\lim_{\Delta\to0}\int(\cdot)\Leftarrow\int\lim_{\Delta\to0}(\cdot)$ [כפי שנראה בשקף]
- (מסגרת כחולה מקווקווה) לכן הגבול החלש תחת סימן האינטגרל: $W_-\lim_{\Delta\to0}P_\Delta\triangleq\delta(t)$; $\int_{-\infty}^\infty\delta(t')dt':=\lim_{\Delta\to0}\int_{-\infty}^\infty P_\Delta(t')dt'=1$

## שקף 33 - Typical Waveforms - The Unit Impulse - מתקף יחידה
- תכונות של $\delta(t)$: $\begin{bmatrix}\delta(t-t_0)=0,\ \forall t\ne t_0\\singular,\ t=t_0\end{bmatrix}$, $\int_{-\infty}^\infty\delta(t-t_0)dt=\int_{t_0^-}^{t_0^+}\delta(t-t_0)dt=1$ [גרף: $\delta(t-t_0)$ symbol]
- עבור כל פונ' $f(t)$ רציפה ב-$t_0$ ואינטגרבילית בסביבת $t_0$: $f(t)\delta(t-t_0)=f(t_0)\delta(t-t_0)\Rightarrow\int_{-\infty}^\infty f(t)\delta(t-t_0)dt=\int_{-\infty}^\infty f(t_0)\delta(t-t_0)dt=f(t_0)\int_{-\infty}^\infty\delta(t-t_0)dt=f(t_0)$
- $\int_{-\infty}^t\delta(t')dt':=u(t)\iff\dfrac{du(t)}{dt}:=\delta(t)\Rightarrow\int_{-\infty}^t\delta(t')dt'=\lim_{\Delta\to0}\int_{-\infty}^tP_\Delta(t')dt'=\begin{cases}t<0\to&0\\t>0\to&\lim_{\Delta\to0}\int_0^\Delta\frac1\Delta dt=1\end{cases}=u(t)$

## שקף 34 - Typical Waveforms - פונקציה מוכללת דלתא (The Unit Impulse)
נרצה לראות שלכל $f(t)$ אינטגרבילית בסביבת האפס, ורציפה באפס מתקיים: $\int_{-\infty}^\infty\delta(t)f(t)dt:=\lim_{\Delta\to0^+}\int_{-\infty}^\infty P_\Delta(t)f(t)dt\Rightarrow\lim_{\Delta\to0^+}\frac1\Delta\int_0^\Delta f(t)dt=f(0)$
- אם $f(t)$ אינטגרבילית לפי רימן בקטע סגור בסביבת $t=0$, אזי $F_0(\Delta)$ פונ' רציפה (אפילו במ"ש) בקטע הפנימי בסביבת האפס. נגדיר: $F_0(\Delta)=\int_0^\Delta f(t)dt$
- אם בנוסף, $f(t)$ גם רציפה ב-$t=0$ (ואינטגרבילית רימן בסביבת האפס), אזי $F_0(t)$ גזירה ב-$t=0$, ומתקיים: $F_0'(0)=f(0)$

## שקף 35 - Typical Waveforms - פונקציה מוכללת דלתא (The Unit Impulse)
אם $f(t)$ אינטגרבילית לפי רימן בסביבת $t=0$, ורציפה ב-$t=0$ אזי: $\lim_{\Delta\to0^+}\int_{-\infty}^\infty P_\Delta(t)f(t)dt=\lim_{\Delta\to0^+}\frac1\Delta\int_0^\Delta f(t)dt:=\lim_{\Delta\to0^+}\frac1\Delta F_0(\Delta)\underbrace{=}_{F_0(0)=0}\lim_{\Delta\to0^+}\dfrac{F_0(\Delta)-F_0(0)}\Delta\underbrace{\Longrightarrow}_{\Delta\to0^+}F_0'(0^+)=f(0)$
ולכן ניתן לרשום, $\lim_{\Delta\to0^+}\int_{-\infty}^\infty f(t)P_\Delta(t)dt=\lim_{\Delta\to0^+}f(0)=f(0)$
עפ"י הגדרת פונ' מוכללת דלתא $\delta(t)\triangleq W_-\lim_{\Delta\to0^+}P_\Delta$, נקבל: (באדום) $\int_{-\infty}^\infty\delta(t)f(t)dt=f(0)$. [גרף: $\delta(t)$ symbol]

## שקף 36 - Typical Waveforms - The Unit Doublet - פונקציה מוכללת דובלט
- $\delta'(t)=\begin{cases}0,&t\ne0\\singular,&t=0\end{cases}$. הסינגולריות סביב האפס היא כזו ש: $\int_{-\infty}^t\delta'(t')dt'=\delta(t)$ ו-$\dfrac{d\delta(t)}{dt}=\delta'(t)$. [גרף: $\delta'(t)$ symbol: חץ כלפי מעלה מצד ימין... כפי שנראה: חץ כחול כלפי מעלה משמאל וכלפי מטה מימין]
- נגדיר את הגבול (החלש) תחת סימן האינטגרל: $\delta'(t)=W_-\lim_{\Delta\to0}\varphi_\Delta'(t)$
- לכל גזירה $f(t)$ עם $f'(t)$ רציפה באפס נקבל: $\int_{-\infty}^\infty\delta'(t')f(t')dt'=\delta(t')f(t')\Big|_{-\infty}^\infty-\int_{-\infty}^\infty\delta(t')f'(t')dt'=-f'(0)$

## שקף 37 - Typical Waveforms
שרשרת: The Unit Ramp $r(t)$ $\to$ (נגזרת) $\frac{dr(t)}{dt}=u(t)$ The Unit Step $u(t)$ $\to$ $\frac{du(t)}{dt}=\delta(t)$ The Unit Impulse $\delta(t)$ $\to$ $\frac{d\delta(t)}{dt}=\delta'(t)$ Doublet $\delta'(t)$. בכיוון ההפוך (אינטגרל): $\int_{-\infty}^tu(t')dt'=r(t)$; $\int_{-\infty}^t\delta(t')dt'=u(t)$; $\int_{-\infty}^t\delta'(t')dt'=\delta(t)$; $\int_{-\infty}^tr(t')dt'=\frac{t^2}2u(t)$.
- $r(t)=\begin{cases}0,&t<0\\t,&0\le t\end{cases}$; $u(t)=\begin{cases}0,&t<0\\1,&t>0\end{cases}$; $\delta(t)=\begin{cases}0,&t\ne0\\singular,&t=0\end{cases}$; $\delta'(t)=\begin{cases}0,&t\ne0\\singular,&t=0\end{cases}$

## שקף 38 - Typical Waveforms
לפעמים נוח להשתמש ברישום אופרטורים:
- אופרטור הנגזרת, $p\triangleq p$: $p[f(t)]=\frac d{dt}f(t)$. אופרטור האינטגרל, $\frac1p\triangleq p^{-1}$: $\frac1p[f(t)]=\int_{-\infty}^tf(t')dt'$. $\Leftarrow$ מוגדר במובן של $p^{-1}p=pp^{-1}=I$ כך ש: $f(-\infty)=0$.
- אופרטור הנגזרת, $D\triangleq D$: $D[f(t)]=\frac d{dt}f(t)$. אופרטור האינטגרל, $\frac1D\triangleq D^{-1}$: $\frac1D[f(t)]=\int_0^tf(t')dt'$. $\Leftarrow$ $DD^{-1}\ne D^{-1}D$. $DD^{-1}f(t)=f(t)\ne D^{-1}Df(t)=f(t)-f(0)$

## שקף 39 - Typical Waveforms - The Unit Impulse - מתקף יחידה
- **משפט פייר Fejér:** תהי נתונה משפחה של פונקציות על $\mathbb R$, $\{\varphi_\Delta(t),\ \Delta\ge0\}$ המקיימת:
  - (1) $\int_{-\infty}^\infty\varphi_\Delta(t)dt=1$, $\varphi_\Delta(t)\ge0$, $\forall\Delta>0,t\in\mathbb R$
  - (2) $\mu_\Delta(\delta)=\sup_{|t|\ge\delta}(\varphi_\Delta(t))\xrightarrow{\Delta\to0}0$, $\forall\delta>0$
  - אזי לכל פונקציה $f(t)$ על $\mathbb R$, רציפה באפס עם $\int_{-\infty}^\infty|f(t')|dt'<\infty$ מתקיים: (מסגרת אדומה) $\lim_{\Delta\to0^+}\int_{-\infty}^\infty\varphi_\Delta(t)f(t)dt=f(0)$
- [גרפים: $P_\Delta(t)$ ו-$\Lambda_\Delta(t)$: מלבן בגובה $1/\Delta$ ומשולש; $\frac1\Delta\Pi\left(\frac t\Delta\right)$ מ-$-\Delta/2$ עד $\Delta/2$]

## שקף 40 - תרגיל – שאלה ממבחנים – פונ' מוכללת $\delta(t)$
נתונה משפחת הפונ' החד פרמטרית $\Lambda_\Delta(t)$ הבאה $\{\Lambda_\Delta(t),\ \Delta>0\}$: [גרף משולש בגובה $1/\Delta$ בין $-\Delta$ ל-$\Delta$] $\Lambda_\Delta(t)=\begin{cases}\frac{t+\Delta}{\Delta^2},&-\Delta<t\le0\\\frac{\Delta-t}{\Delta^2},&0<t<\Delta\\0,&\text{אחרת}\end{cases}$
- הוכיחו כי $W_-\lim_{\Delta\to0}\Lambda_\Delta=\delta(t)$ ביחס למשפחת הפונקציות האינטגרביליות על $\mathbb R$ ורציפות באפס. כלומר, הראו כי לכל $f(t)$ אינטגרבילית על $\mathbb R$ ורציפה באפס, אזי מתקיים: $\lim_{\Delta\to0^+}\int_{-\infty}^\infty\Lambda_\Delta(t)f(t)dt=f(0)$

## שקף 41 - פונ' מוכללת $\delta(t)$ - דרך א'
משפחת הפונ' החד פרמטרית $\Lambda_\Delta(t)$ על $\mathbb R$ מקיימת את משפט פייר.
- (1) $\int_{-\infty}^\infty\Lambda_\Delta(t)dt=1$, $\Lambda_\Delta(t)\ge0$, $\forall\Delta>0,t\in\mathbb R$
- (2) $\mu_\Delta(\delta)=\sup_{|t|\ge\delta}(\Lambda_\Delta(t))\xrightarrow{\Delta\to0}0$ $\Leftarrow$ מכיוון שפונ' המשולש מתאפסת מחוץ לתחום $[-\Delta,\Delta]$; עבור $\Delta<\delta$ לכן $\mu_\Delta(\delta)=0$
- אזי לכל פונ' $f(t)$ אינטגרבילית על $\mathbb R$ ורציפה באפס מתקיים: $\lim_{\Delta\to0^+}\int_{-\infty}^\infty\Lambda_\Delta(t)f(t)dt=f(0)$

## שקף 42 - פונ' מוכללת $\delta(t)$ - דרך ב'
דרך ב': רציפות $f(t)$ בנקודה $t=0$:
- $\forall\varepsilon>0\ \exists\delta>0:\ |t-0|<\delta\Rightarrow|f(t)-f(0)|<\varepsilon$
- אם נבחר $0<\Delta<\delta$ אז לכל $t$ בתחום שבו פונ' המשולש לא אפס: $|t|<\Delta<\delta\Rightarrow|f(t)-f(0)|<\varepsilon$. כלומר: $f(0)-\varepsilon\le f(t)\le f(0)+\varepsilon$, $\forall|t|<\Delta<\delta$
- נכפיל את אי-השוויון בפונ' הדגימה $\Lambda_\Delta(t)$ (שהיא תמיד חיובית): $[f(0)-\varepsilon]\Lambda_\Delta(t)\le f(t)\Lambda_\Delta(t)\le[f(0)+\varepsilon]\Lambda_\Delta(t)$

## שקף 43 - פונ' מוכללת $\delta(t)$ - דרך ב' (המשך)
- נבצע הכללה לאינטגרלים: $[f(0)-\varepsilon]\int_{-\Delta}^\Delta\Lambda_\Delta(t)dt\le\int_{-\Delta}^\Delta\Lambda_\Delta(t)f(t)dt\le[f(0)+\varepsilon]\int_{-\Delta}^\Delta\Lambda_\Delta(t)dt$
- שטח פונ' = 1, ולכן מתקבל: $f(0)-\varepsilon\le\int_{-\Delta}^\Delta\Lambda_\Delta(t)f(t)dt\le f(0)+\varepsilon$, $\forall0<\Delta<\delta$

## שקף 44 - פונ' מוכללת $\delta(t)$ - דרך ב' (סיום)
- לכן, לכל $\varepsilon>0$ שנבחר, קטן כרצוננו $\varepsilon\to0$, קיים $\delta>0$ מתאים, כך שלכל $0<\Delta<\delta$ מתקיים אי-השיוויון. לכן עפ"י כלל הסנדוויץ, נקבל: (מסגרת אדומה) $\lim_{\Delta\to0^+}\int_{-\Delta}^\Delta\Lambda_\Delta(t)f(t)dt=f(0)$
- **לסיכום:** ככל שהמשולש נהיה **צר יותר**, הוא "דוגם" רק את הערכים של $f$ שקרובים ל-$f(0)$, ואז האינטגרל הופך להיות פשוט **הערך של הפונ' $f$ בנקודה הזאת** (בזמן הופעת ההלם).
- מכיוון שזה קורה לכל $f$ אינטגרבילית על $\mathbb R$ ורציפה בנקודה 0, ניתן לומר ש-$\Lambda_\Delta(t)$ מהווה קירוב טוב לפונקציה המוכללת דלתא $\delta(t)$: $\delta(t)=W_-\lim_{\Delta\to0^+}\Lambda_\Delta$

## דברים לבדיקה
- שקף 36: תיאור הדובלט בציור נרשם כפי שנראה (חץ כחול כלפי מעלה משמאל, כלפי מטה מימין).
- שקף 38: האופרטורים נרשמו כפי שנראים (שני סימונים: $p$ ו-$D$).
- שקף 32: הביטויים עם הגבולות והאינטגרלים נרשמו כפי שנראים בשקף; הכיווניות של $\Leftarrow/\not\Rightarrow$ קראתי חלקית.
- שקף 24: סעיף 2 מופיע בלי פתרון (השקף מציג את תשובת סעיף 1 בלבד).
