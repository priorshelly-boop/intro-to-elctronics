# תמלול: AH-תרגול 5
מקור: `raw/recitations/AH-תרגול 5.pdf` (23 שקפים מוקלדים, אדיר חזן). תמלול נאמן מקריאה חזותית של השקפים, בלי תיקון והשלמה. `[לא קריא]` = לא נקרא. תיאורי ציורים בסוגריים מרובעים. מספור לפי מספר השקף בכותרת.

## שקף 1
מבוא להנדסת חשמל 361.1.1021. תרגול #5. תשפ"ז סמ' א' (2026/7). אדיר חזן. נושאים: הספק ואנרגיה (נגדים, קבלים, סלילים). קבלים וסלילים לא לינארים.

## שקף 2 - תזכורת: נגדים Resistors
הספק רגעי: $p(t)=v(t)i(t)$. נגד הינו רכיב בעל שני הדקים שבו מתקיים **בכל רגע** קשר בין המתח הנופל עליו לבין הזרם העובר דרכו: $v(t)=f_R(i(t),t)$. העקומה המגדירה את הקשר במישור $vi$ נקראת אופיין הנגד בזמן $t$.
| תכונות | לינארי (Linear) | לא לינארי (Non-Linear) |
|---|---|---|
| קבוע בזמן (TI) | $v(t)=R\,i(t)$ | $v(t)=f_R(i(t))$ |
| משתנה בזמן (TV) | $v(t)=R(t)\,i(t)$ | $v(t)=f_R(i(t),t)$ |
| נגד LTI פאסיבי: $R\ge0$ | $G\equiv\frac1R$, $[G]=\Omega^{-1}=\mho$; $R$ – Resistance, $G$ – Conductance | אופיין הנגד $f_R$ / הקשר $v_Ri_R$ |
| חיבור $N$ נגדים בטור | $R_{eq}=\sum R_k$, $G_{eq}=\left(\sum\frac1{G_k}\right)^{-1}$ | $i_{eq}=i_k$, $v_{eq}=\sum v_k$ |
| חיבור $N$ נגדים במקביל | $R_{eq}=\left(\sum\frac1{R_k}\right)^{-1}$, $G_{eq}=\sum G_k$ | $v_{eq}=v_k$, $i_{eq}=\sum i_k$ |

## שקף 3 - תזכורת: קבלים Capacitors
קבל הינו רכיב בעל שני הדקים שבו מתקיים **בכל רגע** קשר בין המטען על פניו לבין המתח בין הדקיו: $q(t)=f_c(v(t),t)$. העקומה המגדירה את הקשר במישור $qv$ נקראת אופיין הקבל בזמן $t$. $i(t)=\frac{dq(t)}{dt}$
| תכונות | לינארי | לא לינארי |
|---|---|---|
| TI | $q(t)=C\,v(t)$; $i(t)=C\,\dot v(t)$ | $q(t)=f_c(v(t))$; $i(t)=q'(v)\cdot\dot v(t)$ |
| TV | $q(t)=C(t)v(t)$; $i(t)=\dot C(t)v(t)+C(t)\dot v(t)$ | $q(t)=f_c(v(t),t)$; $i(t)=\dot q(t)+q'(v)\dot v(t)$ |
| קבל LTI פאסיבי: $C\ge0$ | $[C]=\left[\frac qv\right]=\frac CV=F$, $S=C^{-1}$ | אופיין הקבל $f_c$ / הקשר $q_cv_c$ |
$C$ – Capacitance | $S$ – Elastance. רכיב בעל זיכרון. נזכור, שהמטען "נטו" הצבור על הקבל הוא 0. $W_{t_1\to t_2}:=\Delta E_E(t)\triangleq\int_{q(t_0)}^{q(t)}\hat v(q_1)dq_1$

## שקף 4 - תזכורת: סלילים Inductors
סליל (משרן) הינו רכיב בעל שני הדקים שבו מתקיים **בכל רגע** קשר בין השטף המגנטי הסורר בו לבין הזרם דרכו: $\phi(t)=f_L(i(t),t)$. העקומה המתארת את הקשר $\phi i$ בכל רגע נקראת אופיין הסליל. $v(t)=\frac{d\phi_M(t)}{dt}$
| תכונות | לינארי | לא לינארי |
|---|---|---|
| TI | $\phi(t)=L\,i(t)$; $v(t)=L\,i'(t)$ | $\phi(t)=f_L(i(t))$; $v(t)=\phi'(i)i'(t)$ |
| TV | $\phi(t)=L(t)i(t)$; $v(t)=L'(t)i(t)+L(t)i'(t)$ | $\phi(t)=f_L(i(t),t)$; $v(t)=\phi'(t)+\phi'(i)i'(t)$ |
| סליל LTI פאסיבי: $L\ge0$ | $[L]=\left[\frac\phi i\right]=\frac{Wb}A=H$, $r=L^{-1}$ | אופיין הסליל $f_L$ / הקשר $\phi_Li_L$ |
$L$ – Inductance | $r$ – Reciprocal Inductance. רכיב בעל זיכרון. נזכור, מחוק פאראדיי (כאשר המתח נמדד לפי כיווני היחוס): $v(t)=\frac{d\phi_M(t)}{dt}$. $W_{t_1\to t_2}:=\Delta E_M(t)\triangleq\int_{\phi(t_1)}^{\phi(t_2)}\hat i(\phi')d\phi'$

## שקף 5 - תזכורת: LTI Capacitor & Inductor
- חיבור קבלים **בטור** מתנהג כמו חיבור נגדים **במקביל**, וחיבור קבלים **במקביל** מתנהג כמו חיבור נגדים **בטור**.
  - חיבור $N$ קבלי LTI בטור: $\frac1{C_{eq}}=\sum_{k=1}^N\frac1{C_k}$, $v_{eq}(t_0)=\sum_{k=1}^Nv_{c_k}(t_0)$
  - חיבור $N$ קבלי LTI במקביל: $C_{eq}=\sum_{k=1}^NC_k$, $v_{eq}(t_0)=v_{c_k}(t_0)$
- חיבור סלילים **בטור/מקביל** מתנהג כמו חיבור נגדים **בטור/מקביל**.
  - חיבור $N$ סלילי LTI בטור: $L_{eq}=\sum_{k=1}^NL_k$, $i_{eq}(t_0)=i_{L_k}(t_0)$
  - חיבור $N$ סלילי LTI במקביל: $\frac1{L_{eq}}=\sum_{k=1}^N\frac1{L_k}$, $i_{eq}(t_0)=\sum_{k=1}^Ni_{L_k}(t_0)$

## שקף 6 - הספק ואנרגיה - Instantaneous Power & Energy
- **הספק רגעי:** $[p]=\left[\frac wt\right]=\frac J{sec}=W$; $p:=\dfrac{dw}{dt}=\dfrac{dw}{dq}\dfrac{dq}{dt}\to p(t)=v(t)i(t)$
- רכיב צורך אנרגיה (למשל נגד פאסיבי, צרכן / עומס): $p(t)=v(t)i(t)>0$ [ציור: רכיב עם $i(t)$, $+v(t)-$]
- רכיב מספק אנרגיה למעגל (למשל מקור, רכיב אקטיבי): $p(t)=-v_s(t)\,i_s(t)<0$ כאשר המקור מספק אנרגיה $v_s,\ i_s>0$ וההספק הנקלט שלו שלילי. [ציור: מקור מתח $v_s(t)$ עם $i_s(t)$]
- **העבודה:** סך כל ההספק בפרק זמן מסויים $\Leftarrow$ העבודה בפרק זמן מסויים $[t_1,t_2]$ היא הפרש האנרגיות: $W_{t_0\to t}:=\int_{t_0}^tp(t')dt'=\int_{t_0}^tv(t')i(t')dt'$. האנרגיה הנקלטת ברכיב עשויה להיאגר בו (למשל קבל / סליל), להתפזר כחום (למשל נגד) או לעבור בין המעגל למקור אנרגיה אחר (למשל מקור מתח), בהתאם לסוג הרכיב.

## שקף 7 - הספק הנכנס לנגד - Power Entering a Resistor, Passivity
- עבור נגד **לינארי**, כאשר $v(t)=R(t)\,i(t)$, ההספק הרגעי המתפזר על הנגד: $p(t):=v(t)\,i(t)\Rightarrow p(t)=\dfrac{v^2(t)}{R(t)}=R(t)\,i^2(t)$ [ציור: נגד $i_R$, $+v_R-$]
- הנגד פאסיבי ($p(t)\ge0$) אם ורק אם $R(t)\ge0$, $\forall t$. כלומר, נגד יהיה פאסיבי אם ורק אם האופיין שלו עובר ברביע ה-I וברביע ה-III כך ש: $v(t)i(t)>0$. [גרף: אופיין עולה דרך הראשית, נקודה $(i(t),v(t))$ עם $i_0,v_0$]
- האנרגיה המתבזבזת על נגד לינארי $R(t)$ בפרק הזמן $[t_1,t_2]$: $W_{t_0\to t}:=\int_{t_0}^tp(t')dt'=\int_{t_0}^tv(t')i(t')dt'=\int_{t_0}^t\frac{v^2(t')}{R(t')}dt'=\int_{t_0}^ti^2(t')R(t')dt'$
- עבור נגד LTI: $v(t)=R\,i(t)\overset{R\ LTI}{\Longrightarrow}W^R_{t_0\to t}=\frac1R\int_{t_0}^tv^2(t')dt'=R\int_{t_0}^ti^2(t')dt'$

## שקף 8 - תרגיל - ההספק המתפזר בנגד
עבור המעגל הבא, [מעגל: $v_{in}$, $R$ ו-$R_L$ בטור] 1) מצאו את ערכו של $R_L$ עבור העברת הספק מקס' לעומס. 2) מהי יעילות המערכת עבור ערך זה?

## שקף 9 - תרגיל - ההספק המתפזר בנגד (סעיף 1)
- $P_{load}=i^2R_L=\left(\dfrac{v_{in}}{R+R_L}\right)^2R_L$
- $P_{max}\Rightarrow\dfrac{dP_{load}}{dR_L}=0,\ \dfrac{d^2P_{load}}{dR_L^2}<0$
- $P_{max}=\max(P_{load})=\max\left(\dfrac{v_{in}^2}{(R+R_L)^2/R_L}\right)\overset{v_{in}=const}{\Longrightarrow}\min\left((R+R_L)^2/R_L\right)$
- $D_{min}\Rightarrow\dfrac{dD}{dR_L}=0,\ \dfrac{d^2D}{dR_L^2}>0$
- $\dfrac{dD}{dR_L}=0\Rightarrow\dfrac d{dR_L}\left(\dfrac{R^2}{R_L}+2R+R_L\right)=-R^2R_L^{-2}+0+1=0\Rightarrow R^2R_L^{-2}=1\Rightarrow R_L=\pm R\overset{R,R_L>0}{\Longrightarrow}$ (מסגרת אדומה) $R_L=R$
- $\dfrac{d^2D}{dR_L^2}>0\Rightarrow\dfrac d{dR_L}(-R^2R_L^{-2}+1)=2R^2R_L^{-3}\Rightarrow2R^2R_L^{-3}>0,\ \forall R,R_L>0$
- $\Rightarrow(R+R_L)^2/R_L$ is min $\Rightarrow\dfrac{v_{in}^2}{(R+R_L)^2/R_L}$ is max $\Rightarrow P_{load}$ is max when $R_L=R\Rightarrow P_{max}=\dfrac{v_{in}^2}{4R_L}$

## שקף 10 - תרגיל - ההספק המתפזר בנגד (סעיף 2)
2) מהי יעילות המערכת עבור ערך זה? $P_{load}=v_Li_L=i^2R_L=\left(\dfrac{v_{in}}{R+R_L}\right)^2R_L\Rightarrow P_{max}=\dfrac{v_{in}^2}{4R_L}$. $P_{Total}=v\,i$. (באדום) $P_{max}\overset{R,R_L>0}{\Longrightarrow}$ (מסגרת אדומה) $R_L=R$. (השקף מסתיים בלי חישוב היעילות.)

## שקף 11 - האנרגיה האצורה בקבל - Energy Stored in Time-Invariant Capacitors
- הזרם דרך הקבל: $i(t)=\dfrac{dq(t)}{dt}$. נניח שאופיין קבל קבוע בזמן (TI) מתואר ע"י הפונ': $v_c=\hat f_c(q)$. $q(t)=f_c(v(t))$ [גרף: $q$ מול $v$, נקודה $(q(t),v(t))$]
- $W_{t_0\to t}:=\int_{t_0}^tp(t')dt'=\int_{t_0}^tv(t')i(t')dt'\Rightarrow\left[\begin{matrix}i(t)dt=dq\\t_0\to q(t_0),t\to q(t)\end{matrix}\right]=\int_{q(t_0)}^{q(t)}v_c(q')dq'$
- האנרגיה האצורה בקבל בזמן $t$: $W^C_{t_0\to t}:=\Delta E_E=E(t)-E(t_0)\xrightarrow{\text{uncharged }q(t_0)=0}E_E(t)=\int_0^{q(t)}v_c(q')dq'$

## שקף 12 - האנרגיה האצורה בקבל - Energy Stored in LTI Capacitors
- נניח שאופיין קבל קבוע בזמן (TI) מתואר ע"י הפונ': $v_c=\hat f_c(q)$. $W_{t_0\to t}:=\int_{t_0}^tp\,dt'=\int v\,i\,dt'\Rightarrow\int_{q(t_0)}^{q(t)}v_c(q')dq'$
- עבור קבל לינארי וקבוע בזמן LTI (פאסיבי אם ורק אם $C>0$), כאשר אופיין הקבל נתון ע"י הקשר: $q(t)=C\,v(t)$:
  - $\Delta E_E:=\int_{q(t_0)}^{q(t)}v_c(q')dq'=\int_{q(t_0)}^{q(t)}\dfrac{q'}C\,dq'=\dfrac12\dfrac{[q^2(t)-q^2(t_0)]}C\overset{C\ LTI}{\Longrightarrow}\Delta E_E=\dfrac12C[v^2(t)-v^2(t_0)]$ (באדום; $q(t)=C\,v(t)$)
- בעזרת קשר זרם-מתח של הקבל: $\Delta E_E:=\int_{t_0}^tp(t')dt'=\int_{t_0}^tv(t')i(t')dt'\Rightarrow\left[\begin{matrix}i(t)dt=Cdv\\t_0\to v(t_0),t\to v(t)\end{matrix}\right]=C\int_{v(t_0)}^{v(t)}v'dv'=\dfrac12C[v^2(t)-v^2(t_0)]$

## שקף 13 - האנרגיה האצורה בסליל - Energy Stored in Time-Invariant Inductors
- המתח על פני הסליל: $v_L(t)=\dfrac{d\phi}{dt}$. נניח שאופיין סליל קבוע בזמן (TI) מתואר ע"י הפונ': $i=\hat f_L(\phi)$. $\phi(t)=f_L(i(t))$ [גרף: $\phi$ מול $i$, נקודה $(i(t),\phi(t))$]
- $W_{t_0\to t}:=\int p\,dt'=\int v\,i\,dt'\Rightarrow\left[\begin{matrix}v(t)dt=d\phi\\t_1\to\phi(t_0),t\to\phi(t)\end{matrix}\right]=\int_{\phi(t_0)}^{\phi(t)}i_L(\phi')d\phi'$
- האנרגיה האצורה בסליל בזמן $t$: $W^L_{t_0\to t}:=\Delta E_M=E(t)-E(t_0)\xrightarrow[\text{initially flux}]{\text{uncharged }\phi(t_0)=0}E_M(t)=\int_0^{\phi(t)}i_L(\phi')d\phi'$

## שקף 14 - האנרגיה האצורה בסליל - Energy Stored in LTI Inductors
- נניח שאופיין סליל קבוע בזמן (TI) מתואר ע"י הפונ': $i_L=\hat f_L(\phi)$. $W_{t_0\to t}:=\int p\,dt'\Rightarrow\int_{\phi(t_0)}^{\phi(t)}i_L(\phi')d\phi'$
- עבור סליל לינארי וקבוע בזמן LTI (פאסיבי אם ורק אם $L\ge0,\ \forall t$), כאשר אופיין הסליל נתון ע"י הקשר: $\phi(t)=L\,i(t)$:
  - $\Delta E_M:=\int_{\phi(t_0)}^{\phi(t)}i_L(\phi')d\phi'=\int\dfrac{\phi'}L\,d\phi'=\dfrac12\dfrac{[\phi^2(t)-\phi^2(t_0)]}L\overset{L\ LTI}{\Longrightarrow}\Delta E_M=\dfrac12L[i^2(t)-i^2(t_0)]$
- בעזרת קשר זרם-מתח של הסליל: $\Delta E_M:=\int p\,dt'=\int v\,i\,dt'\Rightarrow\left[\begin{matrix}v(t)dt=Ldi\\t_0\to i(t_0),t\to i(t)\end{matrix}\right]=\int_{i(t_0)}^{i(t)}i'L\,di'=\dfrac12L[i^2(t)-i^2(t_0)]$

## שקף 15 - תרגיל - האנרגיה האצורה בסליל ובקבל
עבור המעגלים הבאים, [מעגל קבל: מקור $v_s(t)$ וקבל $C$; מעגל סליל: מקור זרם $i_s(t)$ וסליל $L$]: $v_s(t)=u(t)-u(t-1)$, $C=1$ (F), $q(0^-)=0$; $i_s(t)=u(t)-u(t-1)$, $L=1$ (H), $\phi(0^-)=0$. חשבו את האנרגיה האצורה בסליל ובקבל LTI.

## שקף 16 - תרגיל - האנרגיה האצורה בקבל (פתרון)
- $W^C_{t_0\to t}:=\Delta E_E=\int_{t_0}^tp\,dt'=\int v\,i\,dt'$
- $W^C_{t_0\to t}=\int_0^tp\,dt'=\int_0^tv_c(t')i_c(t')dt'\overset{C\ LTI}{\Longrightarrow}\int_{v(0)}^{v(t)}v_c\,C\,dv_c=\frac12C[v_c^2(t)-v_c^2(0)]\overset{v_s=v_c}{\Longrightarrow}\frac C2v_s^2(t)$
- $\overset{C=1\ F}{\Longrightarrow}\frac12[u(t)-u(t-1)]^2=\frac12[u(t)-u(t-1)]$
- $\Rightarrow E_C=\begin{cases}0,&t<0\\\frac12\ (J),&0<t<1\\0,&1<t\end{cases}$
- $v_s(t)=u(t)-u(t-1)$; $C=1$ (F), $q(0^-)=0$; $\overset{C\ LTI}{\Longrightarrow}v(0)=\frac{q(0)}C=0$

## שקף 17 - תרגיל - האנרגיה האצורה בסליל (פתרון)
- $W_{t_0\to t}:=\Delta E_M=\int p\,dt'=\int v\,i\,dt'$
- $W^L_{t_0\to t}=\Delta E_M=\int_0^tv_L(t')i_L(t')dt'\overset{L\ LTI}{\Longrightarrow}\int_{i(0)}^{i(t)}i_L\,L\,di_L=\frac12L[i_L^2(t)-i_L^2(0)]=\frac L2i_s^2(t)$
- $\overset{L=1\ H}{\Longrightarrow}\frac12[u(t)-u(t-1)]^2=\frac12[u(t)-u(t-1)]$
- $\Rightarrow E_L=\begin{cases}0,&t<0\\\frac12\ (J),&0<t<1\\0,&1<t\end{cases}$
- $i_s(t)=u(t)-u(t-1)$; $L=1$ (H), $\phi(0)=0$; $\overset{L\ LTI}{\Longrightarrow}i(0)=\frac{\phi(0)}L=0$

## שקף 18 - תרגיל (שני קבלים לא לינאריים בטור)
עבור המעגל הבא, האופיינים של 2 קבלים לא-לינארים נתונים ע"י העקומות במישור $qv$. ברגע $t=0$, לפני הפעלת מקור המתח, שני הקבלים לא טעונים, כלומר המטען ההתחלתי: $q_k(0)=0,\ k=\{1,2\}$. האופיינים נמדדים כך: [ציור: קבל 1 עם $v_{c1}$ בין 1 ל-$1'$; קבל 2 עם $v_{c2}$ בין 2 ל-$2'$]. 
1) מצאו את האופיין השקול. 2) מצאו את האנרגיה האצורה במערכת ובכל אחד מהקבלים, כאשר: $v_{in}=1$ V, $v_{in}=-1$ V, $v_{in}=2$ V.
[מעגל: $v_{in}$ בטור עם קבל 1 (מתח $v_1$, קוטביות שלילית למעלה) וקבל 2 (מתח $v_2$)]
- [גרף $q_2(v_2)$: 0 בין $v_2=-1$ ל-0, אחר כך שיפוע 1 לכל כיוון (עבור $v_2>0$ ו-$v_2<-1$)]
- [גרף $q_1(v_1)$: שיפוע 1, קבוע ב-1 עבור $v_1>1$]

## שקף 19 - תרגיל (אופיין שקול)
1) מצאו את האופיין השקול. [גרפים כמו בשקף הקודם, בציר עם ערכים $\pm1,\pm2$] KVL: $-v_{eq}-v_1+v_2=0\Rightarrow$ (מסגרת אדומה) $v_{eq}=v_2-v_1$

## שקף 20 - תרגיל (מטען)
KCL: $i_{c1}+i_{c2}=0\Rightarrow-i_{c1}=i_{c2}$. $-\dfrac{dq_1}{dt}=\dfrac{dq_2}{dt}$; $-[q_1(t)-q_1(0)]=q_2(t)-q_2(0)$. נתון $\Rightarrow q_k(0)=0,\ k=\{1,2\}\Rightarrow$ (מסגרת אדומה) $-q_1(t)=q_2(t)$.
עבור חיבור טורי: KCL: $i_{eq}=-i_{c1}=i_{c2}$. $i(t)=\frac{dq}{dt}\iff q(t)=q(t_0)+\int_{t_0}^ti(t')dt'$

## שקף 21 - תרגיל (בניית האופיין השקול)
- [גרף $q_1(v_{c1})$; גרף $-q_1$ מול $v_{c1}$ (שיקוף); גרף $-q_1$ מול $-v_{c1}$]
- KCL: $\Rightarrow q_{eq}(t)=-q_1(t)=q_2(t)$. KVL: $\Rightarrow v_{eq}(t)=v_2(t)-v_1(t)$ [מעגלים עם $i_{eq}$, $i_{in}$, $-i_{c1}$, $i_{c2}$]

## שקף 22 - תרגיל (בניית האופיין השקול, המשך)
- [גרפים: $q_2(v_2)$, $-q_1$ מול $-v_1$, ו-$q_{eq}(v_{eq})$ ריק]
- KCL: $\Rightarrow q_{eq}(t)=-q_1(t)=q_2(t)$. KVL: $\Rightarrow v_{eq}(t)=v_2(t)+[-v_1(t)]$ [מעגל שקול: קבל יחיד עם $v_{eq}$, $i_{eq}$]

## שקף 23 - תרגיל (אנרגיה)
2) מצאו את האנרגיה האצורה במערכת ובכל אחד מהקבלים, כאשר: $v_{in}=1$ V, $v_{in}=-1$ V, $v_{in}=2$ V. ברגע $t=0$ לפני הפעלת מקור המתח, שני הקבלים לא טעונים. 
- $v_{in}=1$ (V) $\Rightarrow q_2=(-q_1)=\dfrac12$ (C)
- $W^C_{t_0\to t}=\Delta E_E=\int_{t_0}^tp\,dt'=\int v\,i\,dt'=\int_{q(t_0)}^{q(t)}v_c(q')dq'$
- $W^{C_1}_{t_0\to t}=\Delta E_1=\int_0^{-1/2}q_1dq_1=\left.\dfrac{q_1^2}2\right|_0^{-\frac12}=\dfrac18$ (J)
- $W^{C_2}_{t_0\to t}=\Delta E_2=\int_0^{1/2}q_2dq_2=\left.\dfrac{q_2^2}2\right|_0^{\frac12}=\dfrac18$ (J)
- $\Rightarrow W_{total}=W^{C_1}_{t_0\to t}+W^{C_2}_{t_0\to t}=\dfrac14$ (J)
- (השקף מציג רק את המקרה $v_{in}=1$ V.)

## דברים לבדיקה
- שקפים 18–23: אופייני הקבלים נקראו מהגרפים בלבד; נקודות הציר (למשל המדרגה של $q_2$ בין $-1$ ל-0) נרשמו כפי שנראות ואינן מאומתות במספרים.
- שקף 23: חישובי $v_{in}=1$ V בלבד מופיעים; חישובי $-1$ V ו-2 V לא מופיעים.
- שקף 10: חישוב היעילות (סעיף 2 בשקף 8) לא מופיע בשקפים.
