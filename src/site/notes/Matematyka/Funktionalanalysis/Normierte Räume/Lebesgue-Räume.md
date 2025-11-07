---
{"dg-publish":true,"permalink":"/matematyka/funktionalanalysis/normierte-raeume/lebesgue-raeume/","created":"2025-11-07T01:04:23.060+01:00","updated":"2025-11-07T22:41:03.820+01:00"}
---


# HIi

<!--META:
Modified: 2025-11-07 01:19
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=25,26
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!remark|I.1.h]- Unzulänglichkeiten der Riemannschen Integration für Funktionalräume
>  
> **Bei dem Versuch,** analog zu den $\ell^{p}$-[[Matematyka/Funktionalanalysis/Normierte Räume/Normierte Folgenräume#^7f7af8\|Folgenräumen]] **Banachräume integrierbarer Funktionen zu definieren,** <u>stößt man auf große Schwierigkeiten:</u>
> 
> > ***Riemann — $L^1$ — Norm:***
> > 
> > Betrachte zunächst <u>auf $C\left[a, b\right]$ die Riemann — $L^1$ — Norm</u>:
> > 
> > $$\left\|f\vphantom{A}\right\|_{1}= \int_{a}^{b}\left|f\left(t\right)\vphantom{\sum}\right|\ \mathrm{d}t$$
> > 
> > Dann stoßen wir auf das Problem:
> > 
> > > [!example]- Hinweis auf die Unvollständigkeit von $C\left[a, b\right]$ bzgl. der Riemann — $L^1$ — Norm
> > > 
> > > O.E. nehmen wir <u>$a=0 \text{ und } b=2$</u> an und setzen:
> > > 
> > > $$f_{n}\left(t\right) = \cases{t^{n}\quad\,\text{für }\ 0 \leq t \leq 1 \\ 1^{\hphantom{n}}\quad\text{für }\ 1 < t \leq 2}$$
> > > 
> > > Dann ist <u>$\left(f_{n}\right)_{n\,\in\,\mathbb{N}}$ eine Cauchyfolge in ${} C\left[0,2\right]$ bzgl. $\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{1}$,</u> denn:
> > > 
> > > $${\color{gray}\forall_{\large n \geq m}:}\ \left\|f_{n}-f_{m}\vphantom{\sum}\right\|_{1}=\int_{0}^{1}\left(t^{m}-t^{n}\right)\ \mathrm{d}t\ \leq\ \frac{1}{m+1}$$
> > > 
> > > 1. ***Erster Grenzwertkandidat***
> > > 	
> > > 	Die Folge $\left(f_{n}\right)$ scheint nun gegen ein durch:
> > > 	
> > > 	$$f\left(t\right) = \begin{cases} 0 & \text{für } 0 \leq t < 1 \\ 1 & \text{für } 1 \leq t \leq 2 \end{cases}$$
> > > 	
> > > 	definiertes $f$ zu konvergieren, und <u>$f$ ist nicht stetig</u>.
> > > 	​
> > > 2. ***Zweiter Grenzwertkandidat***
> > > 	
> > > 	Mit dem gleichen Recht könnte man $\tilde{f}$ mit:
> > > 	
> > > 	$$\tilde{f}\left(t\right) = \cases{0\quad\text{für }\ 0 \leq t \leq 1 \\ 1\quad\text{für }\ 1 < t \leq 2}$$
> > > 	
> > > 	als <u>«freilich ebenfalls unstetigen»</u> Limes von $\left(f_{n}\right)_{n\,\in\,\mathbb{N}}$ ansehen.
> > > 	​
> > > > *Könnte man vielleicht doch einen Limes in $C\left[0,2\right]$ finden, wenn man nur lange genug sucht? Wir werden uns überlegen, dass das nicht möglich ist:*
> > > 
> > 
> > > [!missing]- Beweis der Unvollständigkeit von $C\left[a, b\right]$ bzgl. der Riemann — $L^1$ — Norm:
> > > 
> > > > [!Help]- Bestimmung eines bzgl. der Riemann — $L^1$ — Norm normierten Oberraums
> > > > 
> > > > - **$R\left[0,2\right]$**
> > > > 	
> > > > 	Zunächst könnte man die <u>Riemann — $L^1$ — Norm</u> auf dem wie folgt definieren:
> > > > 	
> > > > 	$$R\left[0,2\right]:=\left\{g:\left[0,2\right] \rightarrow \mathbb{R}\ \middle|\ g \text{ Riemann-integrierbar auf } \left[0,2\right]\vphantom{\sum} \right\}$$
> > > > 	
> > > > 	<u>Oberraum $R\left[0,2\right]$ von $C\left[0,2\right]$</u> betrachten:
> > > > 	
> > > >     > [!bug]- $\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{1}$ nur eine Halbnorm auf $R\left[0,2\right]$
> > > >     > 
> > > >     > Auf $R\left[0,2\right]$ definiert ***$\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{1}$ aber nur noch eine Halbnorm,*** so dass <u>konvergente Folgen keinen eindeutig bestimmten Limes</u> mehr besitzen.
> > > >     > 
> > > >     > *«Oben hatten wir $f$ und $\tilde{f}$ als Limiten von $\left(f_{n}\right)_{n\,\in\,\mathbb{N}}$ ausgemacht!»*
> > > >     > ​
> > > > 	
> > > > - **$\left\langle \left\{f\right\}\ ,\,C\left[0,2\right]\vphantom{\sum} \right\rangle$**
> > > > 	
> > > > 	Wir betrachten deshalb die <u>lineare Hülle von $\left\{f\right\}$</u> *«$\text{bzw.}\{\tilde{f}\}$»* <u>und $C\left[0,2\right]$</u> und bezeichnen diesen <u>Untervektorraum von $R\left[0,2\right]$</u> mit $X$:
> > > > 	
> > > > 	$$X:=\left\{g+\lambda f\ \middle|\ g \in C\left[0,2\right]\ \wedge\ \lambda \in \mathbb{K}\vphantom{\sum}\right\}$$
> > > > 	
> > > >     > [!success]- Korrektheit der $\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{1}$ Norm auf X
> > > >     > 
> > > >     > ***Auf $X$ ist $\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{1}$ aber eine*** *«ganze»* ***Norm,*** denn:
> > > >     > 
> > > >     > $${\color{gray} \forall_{\large g\, \in\, C\left[0,2\right]\ \wedge\ \lambda\, \in\, \mathbb{K}}: } \ \left\|g+\lambda f\vphantom{A}\right\|_{1}=0\ \ \Longrightarrow\ \ \int_{0}^{1} \left|g\left(t\right){\color{gray}{\tiny+\lambda f=0}}\vphantom{\sum}\right|\ \mathrm{d}t = 0 = \int_{1}^{2}\left|g\left(t\right)+\lambda{\tiny\color{gray}\cdot f=1} \vphantom{\sum} \right|\ \mathrm{d}t$$
> > > >     > 
> > > >     > und <u>wegen der Stetigkeit von $g$ folgt</u> nun:
> > > >     > 
> > > >     > $$g\left(t\right)=\cases{\hphantom{-}0\ \quad \text{für }\ 0 \leq t \leq 1 \\ -\lambda\quad\, \text{für }\ 1 \leq t \leq 2} \quad \Longrightarrow \quad -\lambda=g\left(1\right)=0$$
> > > >     > 
> > > >     > Also ist <u>$\lambda=0 \text{ und } g=0$</u>.
> > > >     > 
> > > >     
> > > 
> > > Jetzt schließen wir, dass <u>$C\left[0,2\right]$ kein bzgl. der Riemann — $L^1$ — Norm abgeschlossener Unterraum des normierten Raums $X$ ist,</u> denn in der Tat hat **die Folge $\left(f_{n}\right)_{n\,\in\,\mathbb{N}}$ den in $X$ eindeutig bestimmten Grenzwert**:
> > > 
> > > $$f\left(t\right) = \begin{cases} 0 & \text{für } 0 \leq t < 1 \\ 1 & \text{für } 1 \leq t \leq 2 \end{cases}\quad \notin \quad C\left[0,2\right]$$
> > > 
> > > und erhalten mit [[Matematyka/Funktionalanalysis/Normierte Räume/Normierte Räume#^da12bb\|Lemma I.1.3 Punkt 2]] die ***Unvollständigkeit von $C\left[0,2\right]$.***
> > > 
> 
> Welche Lösungsansätze könnten wir in diesem Fall vielleicht noch versuchen?
> 
> - Man könnte nun **abstrakt die Vervollständigung definieren** *«vgl. [[Matematyka/Funktionalanalysis/Normierte Räume/Normierte Räume#^07ad09\|Bemerkung I.1.2.ex.1]]»*, das liefert jedoch <u>wenig Aufschluss über die konkrete Gestalt</u> des so erhaltenen Banachraums.
> 	
>     > *z.B. ist nicht klar, ob dessen Elemente als Funktionen aufgefasst werden können, und wenn ja, als welche*
> 	
> - Eine andere Idee wäre es, **${} \left\|\,{\large\cdot}\,\vphantom{A}\right\|_1$ auf $R\left[a, b\right]$ zu definieren und  evtl. auch uneigentlich Riemann-integrierbare Funktionen zuzulassen**. Wie bereits festgestellt, <u>erhält man so nur einen halbnormierten Raum</u>. 
> 	
> 	**Schlimmer noch:** die gewünschte <u>Vollständigkeit stellt sich immer noch nicht ein</u>.
> 	
> 	*«Der erstgenannte Defekt einer Halbnorm lässt sich in der Tat auch bei dem jetzt vorzustellenden Weg nicht vermeiden»*
> 	
> Wir schließen daraus, dass man sich daher ***etwas völlig Neues einfallen lassen muss*** und die wesentliche <u>Neuerung besteht darin, die Lebesguesche Integrationstheorie zu verwenden</u>.
> 
>
{ #070e89}

> 


## Funktion


<!--META:
Modified: 2025-11-07 02:34
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=28,29
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!lemma|I.1.8]- Reihenkriterium der Vollständigkeit
>  
> > [!requirements]-
> >  
> > *Sei $\left(X,\|\cdot\|\vphantom{\sum}\right)$ ein halbnormierter Raum*
> > 
> 
> Für einen **halbnormierten Raum** sind <u>folgende Aussagen äquivalent</u>:
> 
> 1. ***Vollständigkeit des Raumes***
> 	
> 	$$X \text{ ist vollständig}$$
> 	​
> 2. ***Konvergenz aller absolut konvergenten Reihen***
> 	
> 	$$\forall_{\large \left(x_{n}\right)_{n\,\in\,\mathbb{N}}\,\subset\,X}:\ \left(\sum_{n=1}^{\infty}\left\|x_{n}\vphantom{A}\right\|<\infty\right)\ \Longrightarrow\ \left(\exists_{\large x\,\in\,X}: \lim_{N \rightarrow \infty}\left\|x-\sum_{n=1}^{N} x_{n}\right\|=0\right)$$
> 	
> ###### `\start{proof}`
> 
> - ***$1. \Rightarrow 2.$***
> 	
> 	Das ist klar, denn $\left(\sum_{n=1}^{N} x_{n}\right)_{N \in \mathbb{N}}$ ist eine <u>Cauchyfolge im vollständigen Raum</u>.
> 	
> - ***$2. \Rightarrow 1.$***
> 	
> 	Sei <u>$\left(x_{n}\right)_{n\,\in\,\mathbb{N}}$ eine Cauchyfolge und wähle zu $\varepsilon_{k}=2^{-k}$ ein $N_{k} \in \mathbb{N}$</u> mit:
> 	
> 	$$\forall_{\large n, m\, \geq\, N_{k}}:\ \left\|x_{n}-x_{m}\vphantom{A}\right\| \leq 2^{-k}$$
> 	
> 	Daraus ergibt sich die Existenz einer <u>Teilfolge $\left(x_{n_{k}}\right)_{k\, \in\, \mathbb{N}}$ mit</u>:
> 	
> 	$$\forall_{\large k\, \in\, \mathbb{N}}:\ \left\|x_{n_{k+1}}-x_{n_{k}}\vphantom{A}\right\| \leq 2^{-k}$$
> 	
> 	Für <u>$y_{k}:=x_{n_{k+1}}-x_{n_{k}}$ ist also $\textstyle\sum_{k}\left\|y_{k}\vphantom{A}\right\|\ \textless\ \infty$</u> und es ergibt sich: *«Teleskopsumme!»*
> 	
> 	$$\sum_{k=1}^{K} y_{k}=x_{n_{K+1}}-x_{n_{1}}$$
> 	
> 	und Schließlich <u>aus Punkt $2.$ folgt</u>:
> 	
> 	$$\begin{align}\exists_{\large y\,\in\,X}:\ \lim_{K \to \infty}\left\|y-\sum_{k=1}^{K} y_{k}\right\| &= \lim_{K \to \infty}\left\|y-x_{n_{K+1}}+x_{n_{1}}\vphantom{\sum}\right\| \\&= \lim_{K \to \infty}\left\|x-x_{n_{K+1}}\vphantom{\sum}\right\| = 0 \qquad {\small\color{gray}«\text{für } x:=y+x_{n_{1}}»} \\\end{align}$$
> 	
> 	Die <u>Teilfolge ${} \left(x_{n_{K}}\right)_{K\,\in\,\mathbb{N}}$ konvergiert</u> daher tatsächlich <u>gegen ein Grenzwert aus $x \in X$</u> und weil eine Cauchyfolge, die eine konvergente Teilfolge besitzt, selbst konvergiert, **folgt die Konvergenz von $\left(x_{n}\right)_{n\,\in\,\mathbb{N}}$.**
> 	
> `\stop{proof}`
> 
>
{ #2086fe}






<!--META:
Modified: 2025-11-07 01:02
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=26,27
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!exm|I.1.h]- Lebesgue-Funktionenraum
>  
> > [!requirements]-
> >  
> > *Seien:*
> > - *$I \subset \mathbb{R}$ ein Intervall, das:*
> > 	
> >     - *offen, halboffen oder abgeschlossen*
> >     - *beschränkt oder unbeschränkt​*
> > - *$\Sigma$ die $\sigma$-Algebra der Borelmengen auf $I$*
> > - *$\lambda$ das Lebesguemaß*
> > 
> 
> Sei $\mathscr{L}^{p}$ die <u>Menge der für $1 \leq p\, \textless\, \infty$ p-Lebesgue-integrierbaren Funktionen auf $I$</u>: *«beachte: wenn $f$ messbar ist, ist $\left|f\right|^p$ messbar»*
> 
> $$\mathscr{L}^{p}\left(I\right) = \left\{f: I \rightarrow \mathbb{K}\ \middle|\ f \text{ messbar}\ \wedge\ \int_{I}\left|f\right|^{p}\ \mathrm{d}\lambda\ <\infty\right\}$$
> 
> und wir definieren für $f \in \mathscr{L}^{p}\left(I\right)$ die *«diesmal Lebegue»* ***$\mathscr{L}^{p}$-Norm***:
> 
> $$\left\|f\vphantom{A}\right\|_{p}^{\star} = \left(\int_{I}\left|f\right|^{p}\ \mathrm{d}\lambda\right)^{\frac{1}{p}}$$
> 
> > *«Wer möchte, kann das Symbol $\textstyle\int f\ \mathrm{d}\lambda$ durch das traditionellere ${} \textstyle\int f\left(t\right)\ \mathrm{d}t$ ersetzen; das wird im Laufe des Texts des öfteren geschehen»*
> 
> Wir behaupten, dass ${} \left(\mathscr{L}^{p}\left(I\right)\ ,\,\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{p}^{\star}\right) {}$ ein ***vollständiger halbnormierter Raum*** ist.
> 
> ###### `\start{proof}`
> 
> 1. ***$\mathscr{L}^{p}$ ist ein Vektorraum***
> 	
>     > [!assumptions]-
>     > 
> 	> *Seien also $f, g \in \mathscr{L}^{P}\left(I\right)$*
>     > ​
> 	
> 	- **Abgeschlossenheit**​
> 	    
> 		Offensichtlich ist <u>$f+g$ als Summe messbarer Funktionen selbst messbar</u> und außerdem gilt:
> 		
> 		$$\begin{aligned}\int_{I}\left|f+g\right|^{p}\ \mathrm{d}\lambda &\leq \int_{I}\left(\left|f\right|+\left|g\right|\vphantom{\sum}\right)^{p}\ \mathrm{d}\lambda \\&\leq \int_{I}\left(2\cdot \max\left\{\left|f\left(t\right)\right|\ ,\,\left|g\left(t\right)\right|\vphantom{\Large A}\right\}\vphantom{\sum^1}\right)^{p}\ \mathrm{d}\lambda \\&= 2^{p} \int_{I} \max\left\{\left|f\left(t\right)\right|^{p}\ ,\,\left|g\left(t\right)\right|^{p}\vphantom{\Large A}\right\}\ \mathrm{d}\lambda \\&\leq 2^{p}\int_{I}\left(\left|f\left(t\right)\right|^{p}+\left|g\left(t\right)\right|^{p}\vphantom{\sum}\right)\ \mathrm{d}\lambda \\&= 2^{p}\underbrace{ \int_{I}\left|f\right|^{p}\ \mathrm{d}\lambda }_{ <\infty } + 2^{p}\underbrace{ \int_{I}\left|g\right|^{p}\ \mathrm{d}\lambda }_{ <\infty }<\infty\end{aligned}$$
> 		
> 		also <u>$f+g \in \mathscr{L}^{P}\left(I\right)$</u>.
> 	    ​
> 	- **Homogenität**
> 		
> 		Trivial
> 		
> - ***Normeigenschaften von $\left\|\,\cdot\,\vphantom{A}\right\|_{p}$***
> 	
> 	Die <u>Homogenität ist offensichtlich,</u> und da wir nur eine Halbnorm erwarten *«Das Gegenbeispiel zur positiven Definitheit ist die Dirichlet-Funktion»*<u>, bleibt nur noch die Dreiecksungleichung</u>.
> 	
> 	> Diese wird, wie im [[Matematyka/Funktionalanalysis/Normierte Räume/Normierte Folgenräume#^7f7af8\|Beispiel i.i.g; Lebesgue-Folgenraum]], in einem separaten Satz behandelt: [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^f6ca79\|Minkowskische Ungleichung «Version für Funktionen»]] 
> 	
> - ***Vollständigkeit***
>     
>     > [!tldr] 
>     > 
>     > > *Wollte man analog zum $\ell^{p}$-Fall vorgehen, würde man eine Cauchyfolge ${} \left(f_{n}\right)_{n\,\in\,\mathbb{N}} {}$ in $\mathscr{L}^{p}\left(I\right)$ und anschließend für festes $t \in I$ die skalare Folge $\left(f_{n}\left(t\right)\right)_{n\,\in\,\mathbb{N}}$ betrachten.*
>     > > 
>     > > *Im Allgemeinen braucht $\left(f_{n}\left(t\right)\right)_{n\,\in\,\mathbb{N}}$ jedoch nicht zu konvergieren, und man muss einen anderen Weg einschlagen.*
>     > > 
>     > 
>     > Wir werden zeigen, dass **jede bezüglich der $\mathscr{L}^{p}$-Norm absolut konvergente Reihe in $\mathscr{L}^{p}$** ***gegen einen Grenzwert in $\mathscr{L}^{p}$ konvergiert*** und somit <u>nach dem</u> [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^2086fe\|Reihenkriterium der Vollständigkeit]] <u>dieser Raum vollständig</u> ist.
>     > ​
>     
>     > [!assumptions]+
>     > 
>     > *Seien $f_{1}, f_{2}, \ldots \in \mathscr{L}^{p}\left(I\right)$ mit:*
>     > 
>     > *$$a:=\sum_{n=1}^{\infty}\left\|f_{n}\right\|_{p}^{\star}<\infty\tag{**}$$*
>     > 
>     > *Wir betrachte die «evtl. $\infty$-wertige» nichtnegative Funktionen:*
>     > 
>     > *$$\begin{align}\hat{g}: I &\longrightarrow \mathbb{\mathbb{R}}^{+} \\t &\longmapsto \sum_{i=1}^{\infty}\left|f_{i}\left(t\right)\vphantom{\sum}\right|\end{align}$$*
>     > 
>     > *und:*
>     > 
>     > *$$\begin{align}\hat{g}_{n}: I &\longrightarrow \mathbb{\mathbb{R}}^{+} \\t &\longmapsto \sum_{i=1}^{n}\left|f_{i}\left(t\right)\vphantom{\sum}\right|\end{align}$$*
>     > 
>     > > *«Als Summe messbarer Funktionen sind $\widehat{g}$ und $\widehat{g}_{n}$ messbar»*
>     
>     Da <u>$\mathscr{L}^{p}\left(I\right)$ ein Vektorraum ist, gilt es $\widehat{g}_{n} \in \mathscr{L}^{p}\left(I\right)$,</u> sowie **aus der [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^f6ca79\|Minkowskischen Ungleichung]] folgt**:
>     
>     $$\left\|\widehat{g}_{n}\right\|_{p}^{\star} \leq \sum_{i=1}^{n}\left\|f_{\large i}\vphantom{\large A}\right\|_{p}^{\star} \ \leq\, a$$
>     
>     Nach Konstruktion <u>konvergiert $\left(\widehat{g}_{n}^{\,p}\right)_{n\,\in\,\mathbb{N}}$ monoton gegen $\widehat{g}^{\,p}$</u> und der **Satz von Beppo Levi** liefert daher:
>     
>     $$\int_{I} \widehat{g}^{\,p}\ \mathrm{d}\lambda = \lim_{n \rightarrow \infty} \int_{I} \widehat{g}_{n}^{\,p}\ \mathrm{d}\lambda\ \leq\ a^{\,p}$$
>     
>     Insbesondere ist $\widehat{g}^{\,p}$ *«und daher auch $\widehat{g}$»* fast überall endlich. Das bedeutet, dass man <u>nach Abänderung von $\widehat{g}$ auf einer Nullmenge $\mathcal{N} \in \Sigma$ eine reellwertige, messbare Funktion $g$ erhält,</u> für die die folgende Identität fast überall erfüllt ist *«nämlich für $t \in I \setminus \mathcal{N}$»* :
>     
>     $$g\left(t\right)= \sum_{i=1}^{\infty}\left|f_{i}\left(t\right)\vphantom{\sum}\right|$$
>     
>     Also ist <u>$g$ punktweise absolut konvergent,</u> und es folgt *«jetzt geht die Vollständigkeit von $\mathbb{K}$ ein!»* die **Existenz des Grenzwerts**:
>     
>     $${\color{gray} \forall_{\large t \in I \setminus \mathcal{N}}: } \ f\left(t\right):=\sum_{i=1}^{\infty} f_{i}\left(t\right)$$
>     
>     <u>Setzt man noch $f\left(t\right)=0$ für $t \in N$,</u> so hat man eine **messbare Funktion $f: I \rightarrow \mathbb{K}$ definiert**. Die Funktion $f$ ist <u>nach Konstruktion $\left|f\right| \leq \widehat{g}$,</u> *«vgl. Definition von $\widehat{g}$»* also folgt:
>     
>     $$\int_{I}\left|f\right|^{\,p}\ \mathrm{d}\lambda \leq \int_{I} \widehat{g}^{\,p}\ \mathrm{d}\lambda\ <\ \infty$$
>     
>     und somit ***$f \in \mathscr{L}^{p}(I)$*** und es bleibt nur die ***Konvergenz bezüglich der Norm zu zeigen***.
>     
>     > [!attention]- Konvergenz bezüglich der Norm
>     > 
>     > 
>     > **z.Z.:** 
>     > 
>     > $$\sum_{i=1}^{\infty} f_{i}=f\ \text{ bzgl. } \left\|\,{\large\cdot}\,\vphantom{A}\right\|_{p}^{\star}\ \text{ d.h.: }{\color{magenta} \lim_{ \large N \to \infty } } \int_{I}\left|{\sum_{\color{magenta}\large i=N}^{\infty} f_{i}}\right|^{p}\ \mathrm{d}\lambda = 0$$
>     > 
>     > Wir verwenden den **Lebesgueschen majorisierten Konvergenzsatz**:
>     > 
>     > ***
>     > 
>     > Sei <u>$\textstyle\color{magenta} h_{N}=\left|\sum_{i=N}^{\infty} f_{i}\right|^{p}$, dann gilt $\color{magenta}h_{N} \rightarrow 0$ fast überall</u> denn
>     > 
>     > $$h_{N}^{\,-p}\leq \sum_{i=N}^{\infty} \left|f_{i}\vphantom{\sum}\right|=g-g_{N-1}$$
>     > 
>     > und <u>$g_{N-1}$ konvergiert monoton von unten gegen $g$,</u> und schließlich folgt:
>     > 
>     > $$0\ \leq\ h_{N}\ \leq\ \left(\sum_{i=N}^{\infty}\left|f_{i}\vphantom{\sum}\right|\right)^{\,p} \leq\ \widehat{g}^{\,p}$$
>     > 
>     > **Wegen ${} \int_{l} \widehat{g}^{\,p}\ \mathrm{d}\lambda\ \leq\ a^{\,p}$ ist $\widehat{g}^{p}$ integrierbar.** Also <u>impliziert der Lebesguesche Konvergenzsatz</u>:
>     > 
>     > $${\color{magenta} \lim_{N \to \infty}} \int_{I} {\color{magenta}h_{N}}\ \mathrm{d}\lambda = 0$$
>     > 
>     > was **zu zeigen war**.
> 	
> `\stop{proof}`
> 
>
{ #f6d061}

> 

***

<!--META:
Modified: 2025-11-07 01:39
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=27,27
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!theorem|I.1.6]- Höldersche Ungleichung «Version für Funktionen»
>  
> > [!requirements]-
> >  
> > *Seien $\mathscr{L}^{1},\mathscr{L}^{q},\mathscr{L}^{p},\mathscr{L}^{\infty}$ Lebesgue-Funktionenräume auf dem Interval $I$*
> > 
> 
> Für <u>$1<p<\infty$ und $\textstyle q=\frac{p}{p-1}$</u> *«also $\textstyle\frac{1}{p}+\frac{1}{q}=1$»*  gilt:
> 
> $$\forall_{\large f\, \in\, \mathscr{L}^{\Large p}\left(I\right)\ \wedge\ g\, \in\, \mathscr{L}^{\Large q}\left(I\right)}:\ fg \in \mathscr{L}^{1}\\ \wedge\ \left\|fg\vphantom{A}\right\|_{1}^{\star} \leq\left\|f\vphantom{A}\right\|_{p}^{\star}\,\left\|g\vphantom{A}\right\|_{q}^{\star}$$
> 
> ###### `\start{proof}`
> 
> > [!info]+ Youngsche Ungleichung
> > 
> > Wir erinnern zunächst an die <u>„gewichtete Ungleichung vom geometrischen und arithmetischen Mittel”</u>:
> > 
> > $${\color{gray}\forall_{\large \sigma, \tau\, \geq\, 0\ \ \wedge\ \ 0\,<\,r\,<\,1}:}\quad\sigma^{r} \tau^{1-r} \leq r \sigma+\left(1-r\right) \tau\tag{I.2}$$
> > 
> > > [!Help]- Beweis
> > > 
> > > - ***$\sigma=0$ oder $\tau=0$***
> > > 	
> > > 	Trivial
> > > 	​
> > > - ***$\sigma, \tau>0$***
> > > 	
> > > 	Die Aussage ist <u>äquivalent zur Konkavität der Logarithmusfunktion</u> *(Abb. I.1)*:
> > > 	
> > > 	$$\log \left(\sigma^r \tau^{1-r}\right)=r \log \sigma+(1-r) \log \tau \leq \log (r \sigma+(1-r) \tau)$$
> > > 	
> > > 	Eine $C^{2}$ — Funktion $f$ ist aber genau dann <u>konkav, wenn $f^{\prime \prime} \leq 0$ gilt;</u> und die **zweite Ableitung von $\log$ ist $-t^{-2}$,** also in der Tat negativ.
> > > 	
> > > 	![Matematyka/Funktionalanalysis/_attachment/9227ebdb340432d0c70ab2beab20b089_v1.png](/img/user/Matematyka/Funktionalanalysis/_attachment/9227ebdb340432d0c70ab2beab20b089_v1.png)
> 
> > [!assumptions]+
> > 
> > *Zur Abkürzung definieren wir:*
> > 
> > *$$A:=\left(\left\|f\vphantom{A}\right\|_{p}^{\star}\right)^{p} \quad \text{und} \quad B:=\left(\left\|g\vphantom{A}\right\|_{q}^{\star}\right)^q$$*
> > 
> > *Ohne Einschränkung darf angenommen werden, dass $A, B > 0$.*
> > 
> > > *«Ist etwa $A=0$, so ist $f=0$ f.ü. und deshalb auch $f g=0$ f.ü.» *
> > 
> > *****
> > 
> > *Wir schreiben $f\left(t\right)$ und $g\left(t\right)$ für beliebiges $t \in I$ und setzen:*
> > 
> > *$$r := \frac{1}{p} \quad \text{bzw.} \quad 1 - r := \frac{1}{q}$$*
> > 
> > *sowie:*
> > 
> > *$$\sigma := \frac{\left|f\left(t\right)\right|^{p}}{A} \quad \wedge \quad \tau := \frac{\left|g\left(t\right)\right|^{q}}{B}$$*
> 
> <u>Einsetzen der Definitionen in (I.2)</u> liefert:
> 
> $$\left(\frac{\left|f\left(t\right)\right|^{p}}{A}\right)^{\frac{1}{p}}\left(\frac{\left|g\left(t\right)\right|^{q}}{B}\right)^{\frac{1}{q}} \leq \frac{1}{p} \frac{\left|f\left(t\right)\right|^{p}}{A}+\frac{1}{q} \frac{\left|g\left(t\right)\right|^{q}}{B}$$
> 
> und durch <u>Integration über $I$</u> folgt:
> 
> $$\begin{align}\frac{\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda}{A^{\frac{1}{p}} B^{\frac{1}{q}}} &\leq \frac{1}{p} \frac{\int_{I}\left|f\left(t\right)\right|^{p}\ \mathrm{d}\lambda}{A}+\frac{1}{q} \frac{\int_{I}\left|g\left(t\right)\right|^{q}\ \mathrm{d}\lambda}{B} \\&\,\Updownarrow \\\frac{\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda}{\left( \left(\left\|f\vphantom{A}\right\|_{p}^{\star}\right)^{p} \right)^{\frac{1}{p}} \left( \left(\left\|g\vphantom{A}\right\|_{q}^{\star}\right)^{q}\right)^{\frac{1}{q}}} &\leq \frac{1}{p} \frac{\int_{I}\left|f\left(t\right)\right|^{p}\ \mathrm{d}\lambda}{\left(\left\|f\vphantom{A}\right\|_{p}^{\star}\right)^{p}}+\frac{1}{q} \frac{\int_{I}\left|g\left(t\right)\right|^{q}\ \mathrm{d}\lambda}{\left(\left\|g\vphantom{A}\right\|_{q}^{\star}\right)^{q}} \\ &\,\Updownarrow \\\frac{\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda}{\left\|f\vphantom{A}\right\|_{p}^{\star} \,\left\|g\vphantom{A}\right\|_{q}^{\star}} &\leq \frac{1}{p} \frac{\int_{I}\left|f\left(t\right)\right|^{p}\ \mathrm{d}\lambda}{\left(\left(\int_{I}\left|f\left(t\right)\right|^{p}\ \mathrm{d}\lambda\right)^{\frac{1}{p}}\right)^{p}}+\frac{1}{q} \frac{\int_{I}\left|g\left(t\right)\right|^{q}\ \mathrm{d}\lambda}{\left(\left(\int_{I}\left|g\left(t\right)\right|^{q}\ \mathrm{d}\lambda\right)^{\frac{1}{q}}\right)^{q}} \\ &\,\Updownarrow \\ \frac{\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda}{\left\|f\vphantom{A}\right\|_{p}^{\star} \,\left\|g\vphantom{A}\right\|_{q}^{\star}} &\leq \frac{1}{p}+\frac{1}{q}=1 \\&\,\Updownarrow \\\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda &\leq {\left\|f\vphantom{A}\right\|_{p}^{\star} \,\left\|g\vphantom{A}\right\|_{q}^{\star}}\end{align}$$
> 
> Schließlich folgt das gewünschte Resultat:
> 
> $$\left\|fg\vphantom{A}\right\|_{1}^{\star} =\int_{I}\left|f\left(t\right) \cdot g\left(t\right)\right|\ \mathrm{d}\lambda \leq {\left\|f\vphantom{A}\right\|_{p}^{\star}\, \left\|g\vphantom{A}\right\|_{q}^{\star}}$$
> 
> `\stop{proof}`
> 
>
{ #8ca550}






<!--META:
Modified: 2025-11-07 02:30
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=27,28
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!corollary|I.1.7]- Minkowskische Ungleichung «Version für Funktionen»
>  
> > [!requirements]-
> > 
> > *Sei $\mathscr{L}^{p}$ ein Lebesgue-Lebesgue-Funktionenraum*
> > 
> 
> Für alle <u>$f, g\, \in\, \mathscr{L}^{p}\left(I\right)\ \text{ und }\ 1 \leq p\,\textless\,\infty$,</u> gilt:
> $$\left\|f+g\vphantom{A}\right\|_{p}^{\star} \leq \left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}$$
> ###### `\start{proof}`
> 
> > [!assumption|s]
> >
> > *Der Fall $p=1$ ist trivial, daher nehmen wir $p>1$ an und statt der Minkowskischen zeigen wir die dazu äquivalente Ungleichung:*
> > 
> > *$$\left(\left\|f+g\vphantom{A}\right\|_{p}^{\star}\right)^{p} \leq\left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right)\left(\left\|f+g\vphantom{A}\right\|_{p}^{\star}\right)^{p-1}$$*
> > 
> > *Dazu schreiben wieder ${} f\left(t\right)\ \text{und}\ g\left(t\right) {}$ für beliebiges $t \in I$.*
> 
> <u>Für $\textstyle\frac{1}{p}+\frac{1}{q}=1$</u> *«also $\textstyle q=\frac{p}{p-1}$»* gilt nach der [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^8ca550\|Hölderschen Ungleichung «Version für Funktionen»]]:
> 
> $$\begin{aligned}
> \left(\left\|f+g\vphantom{A}\right\|_{p}^{\star}\right)^{p}
> &= \int_{I}\left|f\left(t\right)+g\left(t\right)\right|^{p}\ \mathrm{d}\lambda \\
> &\leq \int_{I}\left|f\left(t\right)\right|\cdot\left|f\left(t\right)+g\left(t\right)\right|^{p-1}\ \mathrm{d}\lambda+\int_{I}\left|g\left(t\right)\right|\cdot\left|f\left(t\right)+g\left(t\right)\right|^{p-1}\ \mathrm{d}\lambda \\
> &= \left\|\left|f\right|\cdot\left|f+g\right|^{p-1}\vphantom{\large\sum}\right\|_{1}^{\star} + \left\|\left|g\right|\cdot\left|f+g\right|^{p-1}\vphantom{\large\sum}\right\|_{1}^{\star} \\
> &\leq \left\|f\vphantom{A}\right\|_{p}^{\star}\cdot \left\|\left|f+g\right|^{p-1}\vphantom{A}\right\|_{q}^{\star} + \left\|g\vphantom{A}\right\|_{p}^{\star}\cdot \left\|\left|f+g\right|^{p-1}\vphantom{A}\right\|_{q}^{\star} \\
> &= \left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right)\left\|\left|f+g\right|^{p-1}\vphantom{A}\right\|_{q}^{\star} \\
> &= \left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right) \left(\int_{I}\left|f+g\right|^{\left(p-1\right)q}\ \mathrm{d}\lambda\right)^{\frac{1}{q}} \\
> &= \left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right) \left(\int_{I}\left|f+g\right|^{\left(p-1\right)\frac{p}{p-1}}\ \mathrm{d}\lambda\right)^{\frac{p-1}{p}} \\
> &= \left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right) \left(\left(\int_{I}\left|f+g\right|^{p}\ \mathrm{d}\lambda\right)^{\frac{1}{p}}\right)^{p-1} \\
> &= \left(\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}\right) \left(\left\|f+g\right\|^{\star}_{p}\right)^{p-1}
> \end{aligned}
> $$
> 
> `\stop{proof}`
> 
>
{ #f6ca79}






<!--META:
Modified: 2025-11-07 02:23
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=28,28
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!corollary|I.1.7.ex.1]- Alternativer Beweis der Minkowski-Ungleichung «Version für Funktionen» ohne Hölder-Ungleichung
>  
> Es gibt einen <u>alternativen Beweis</u> für die [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^f6ca79\|Minkowskische Ungleichung «Version für Funktionen»]], der <u>ohne Anwendung der Hölderschen Ungleichung</u> auskommt.
> 
> > [!hint] Konvexität statt Hölder
> >
> > Stattdessen ***nutzt man die Konvexität der Funktion***:
> >
> > $$\varphi_{p}: t \longmapsto \left|t\right|^{p}$$
> >
> > ***für $p \geq 1$***.
> >
> 
> ###### `\start{proof}`
> 
> 1. ***Spezialfall***
> 	
> 	Zuerst wird folgender Spezialfall gezeigt:
> 	
> 	$$\forall_{\large 0\, \leq\, \lambda\, \leq\, 1}:\ \left\|f\vphantom{A}\right\|_{p}^{\star}=\left\|g\vphantom{A}\right\|_{p}^{\star}=1 \quad\Longrightarrow\quad \left\|\lambda f+\left(1-\lambda\right) g\right\|_{p}^{\star} \leq 1$$
> 	
>     > **Argument**
>     > 
>     > Zum Beweis hierfür <u>betrachten wir $f,g \in \mathscr{L}^{p}\left(I\right)$</u> und ***schätzen mit Hilfe der Konvexität von $\varphi_{p}$ ab***:
>     > 
>     > $$\begin{aligned}\left\|\lambda f + \left(1 - \lambda g\right) \right\|_{p}^{\star\,p}&= \int_{I} \left| \lambda f\left(t\right) + \left(1 - \lambda\right) g\left(t\right) \right|^{p}\, \mathrm{d}t \\&= \int_{I} \varphi_{p}\left(\lambda f\left(t\right) + \left(1 - \lambda\right) g\left(t\right)\right)\, \mathrm{d}t \\&\stackrel{\text{Konv.}}{\leq} \int_{I} \left( \lambda\, \varphi_{p}\left(f\left(t\right)\right) + \left(1 - \lambda\right)\, \varphi_{p}\left(g\left(t\right)\right)\right)\, \mathrm{d}t \\&= \lambda \int_{I} \left|f\left(t\right)\right|^{p}\, \mathrm{d}t + \left(1 - \lambda\right) \int_{I} \left|g\left(t\right)\right|^{p}\, \mathrm{d}t \\&= \lambda \left\|f\vphantom{A}\right\|_{p}^{\star\,p} + \left(1 - \lambda\right)\left\|g\vphantom{A}\right\|_{p}^{\star\,p} \\&= \lambda + \left(1 - \lambda\right) = 1\end{aligned}$$
>     > 
>     
> 2. ***Allgemeiner Fall***
> 	
> 	Offenbar kann <u>$f \neq 0, g \neq 0$ angenommen</u> werden und wir setzen:
> 	
> 	$$\tilde{f}=\frac{f}{\left\|f\vphantom{A}\right\|_{p}^{\star}} \quad\wedge\quad \tilde{g}=\frac{g}{\left\|g\vphantom{A}\right\|_{p}^{\star}}$$
> 	
> 	Dann gilt offenbar:
> 	
> 	$$\begin{align}\left\|\tilde{f}\right\|_{p}^{\star}= \left\| \frac{1}{\left\|{f}\vphantom{A}\right\|_{p}^{\star}}\cdot f \right\|_{p}^{\star}&= \frac{1}{\left\|{f}\vphantom{A}\right\|_{p}^{\star}}{\left\|{f}\vphantom{A}\right\|_{p}^{\star}}= 1 \\ \\ &\text{und} \\ \\ \left\|\tilde{g}\right\|_{p}^{\star}= \left\| \frac{1}{\left\|{g}\vphantom{A}\right\|_{p}^{\star}}\cdot g \right\|_{p}^{\star}&= \frac{1}{\left\|{g}\vphantom{A}\right\|_{p}^{\star}}{\left\|{g}\vphantom{A}\right\|_{p}^{\star}}= 1\end{align}$$
> 	
> 	und wir <u>definieren $\lambda, \left(1 - \lambda\right) \in \left[0, 1\right]$</u> wie folgt:
> 	
> 	$$\lambda:=\frac{\left\|f\vphantom{A}\right\|_{p}^{\star}}{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}} \quad\wedge\quad 1-\lambda:=\frac{\left\|g\vphantom{A}\right\|_{p}^{\star}}{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}}$$
> 	
> 	Der bereits bewiesene <u>Spezialfall liefert die gesuchte Abschätzung</u>:
> 	
> 	$$\begin{aligned}1 \geq \left\|\lambda \tilde{f}+\left(1-\lambda\right) \tilde{g}\vphantom{\sum}\right\|_{p}^{\star} &= \left\|\frac{f+g}{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}}\vphantom{A}\right\|_{p}^{\star} \\ &= \frac{1}{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}}\left\|f+g\vphantom{A}\right\|_{p}^{\star} \\&= \frac{\left\|f+g\vphantom{A}\right\|_{p}^{\star}}{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}} \\ &\Updownarrow \\{\left\|f\vphantom{A}\right\|_{p}^{\star}+\left\|g\vphantom{A}\right\|_{p}^{\star}}&\geq{\left\|f+g\vphantom{A}\right\|_{p}^{\star}}\end{aligned}$$
> 	
> 	was zu zeigen war.
> 	
> `\stop{proof}`
> 
>
{ #471ae4}


## Quotienten

<!--META:
Modified: 2025-11-07 01:02
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=30,30
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!lemma|I.1.9]- Faktorisierung halbnormierter Räume durch den Nullraum
>  
> > [!requirements]-
> >  
> > *Sei $\left(X, \left\|\,{\large\cdot}\,\vphantom{A}\right\|^{\star}\right)$ ein halbnormierter Raum*
> > 
> 
> In einem **halbnormierten Raum** gelten folgende Aussagen:
> 
> 1. ***Der Entartungsraum einer Halbnorm ist ein linearer Unterraum***
> 	
> 	$$\mathcal{N}:=\left\{x \in X\ \middle|\ \left\|x\vphantom{A}\right\|^{\star}=0\right\} \text{ ist ein Untervektorraum von } X$$
> 	
> 2. ***Die induzierte Quotientennorm macht den Faktorraum zum normierten Raum***
> 	
> 	$$\left\|{\left[x\right]}\vphantom{\sum}\right\|:=\left\|x\vphantom{A}\right\|^{\star} \text{ definiert eine Norm auf } X\,/\,\mathcal{N}$$
> 	
> 3. ***Vollständigkeit bleibt unter Faktorisierung erhalten***
> 	
> 	$$X \text{ vollständig }\ \Rightarrow\ X\, /\, \mathcal{N} \text{ Banachraum}$$
> 	
> ###### `\start{proof}`
> 
> 4. ***Der Entartungsraum einer Halbnorm ist ein linearer Unterraum***
> 	
> 	Trivial
> 	​
> 5. ***Die induzierte Quotientennorm macht den Faktorraum zum normierten Raum***
> 	
> 	Zunächst <u>mache man sich klar, dass $\left\|\left[x\right]\vphantom{\sum}\vphantom{A}\right\|=\left\|x\vphantom{A}\right\|^{\star}$ wohldefiniert</u> ist *«d.h. nicht vom Repräsentanten der Äquivalenzklasse $\left[x\right]$ abhängt»*.
> 	
>     > [!Help]- Beweis der Unabhängigkeit vom Repräsentanten
>     > 
>     > Ist <u>$x\neq x^{\prime} \in \left[x\right]$,</u> also:
>     > 
>     > $$x^{\prime}=x+n \quad {\color{gray}\text{für}\ n \in \mathcal{N} :=\left\{y \in X \ \middle|\ \left\|y\vphantom{A}\right\|^{\star}=0\vphantom{\sum}\right\}}$$
>     > 
>     > dann gilt <u>$\left\|x^{\prime}\right\|^{\star}=\|x\|^{\star}$, denn aus der Dreiecksungleichung in $X$ folgen</u> beide Richtungen:
>     > 
>     > $$\left\|x^{\prime}\right\|^{\star}= \left\|x+n\vphantom{A}\right\|^{\star} \leq \left\|x\vphantom{A}\right\|^{\star} + \left\|n\vphantom{A}\right\|^{\star}= \left\|x\vphantom{A}\right\|^{\star}$$
>     > 
>     > und ebenso:
>     > 
>     > $$\left\|x\vphantom{A}\right\|^{\star}= \left\|x^{\prime}-n\right\|^{\star} \leq \left\|x^{\prime}\right\|^{\star} + \left\|n\vphantom{A}\right\|^{\star} = \left\|x^{\prime}\right\|^{\star}$$
>     > 
>     > Also <u>schließlich tatsächlich $\left\|x\vphantom{A}\right\|^{\star} = \left\|x^{\prime}\right\|^{\star}$</u>.
>     > ​
> 	
> 	Die **Homogenität und Dreiecksungleichung** <u>folgen dann unmittelbar aus den entsprechenden Eigenschaften von $\left\|\,{\large\cdot}\,\vphantom{A}\right\|^{\star}$</u> und schließlich die **Positive Definitheit**:
> 	
> 	$$\left\|{\left[x\right]}\vphantom{\sum}\right\| = 0\ \ \Longleftrightarrow\ \ x \in \mathcal{N}\ \ \Longleftrightarrow\ \ \left[x\right]=\left[0\right]$$
> 	​
> 6. ***Vollständigkeit bleibt unter Faktorisierung erhalten***
> 	
> 	**Bemerke nur:** 
> 	
>     > Bildet die **Folge der Klassen $\left(\left[x_{n}\right]\vphantom{\sum}\right)_{n\,\in\,\mathbb{N}}$ eine Cauchy- bzw. konvergente Folge**, so <u>gilt dies auch für die Folge $\left(x_{n}\right)_{n\,\in\,\mathbb{N}}$ der Repräsentanten</u> und umgekehrt.
> 	
> `\stop{proof}`
> 
>
{ #e371d3}

> 





<!--META:
Modified: 2025-11-07 20:17
DocTitle: Funktionalanalysis - Dirk Werner
Page: page=30,30
Md5: 604d2bae94bb1307ba73bf712ced1cb85815bfaf597354d324ac2d45870f9262
-->

> [!exm|I.1.h]- Lebesgue-Quotientenraum
>  
> > [!bug]+ Uneindeutigkeit der Konvergenz im Lebesgue-Funktionenraum $\mathscr{L}^{p}\left(I\right)$
> > 
> > Nach [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^f6d061\|Beispiel I.1.h]] ist der Lebesgue-Funktionenraum $\mathscr{L}^{p}\left(I\right)$ als <u>vollständiger halbnormierter Raum</u> ausgewiesen.
> > 
> > > ***Limiten*** sind in diesem Raum jedoch ***nicht mehr eindeutig bestimmt,*** sondern nur noch <u>modulo Elementen des Kerns der Halbnorm $\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{p}^{\star}$,</u> nämlich:
> > > 
> > > $$\mathcal{N}_{p}:=\left\{f\ \in\ \mathscr{L}\left(I\right)\ \middle|\ f=0\ \text{fast überall} \vphantom{\sum}\right\}$$
> > > 
> > > *«Beachte, dass $N_{p}$ in Wirklichkeit gar nicht von $p$ abhängt!»*
> > 
> > Es liegt daher nahe, ***Funktionen zu identifizieren, die fast überall übereinstimmen***:
> > 
> > *«Das angemessene mathematische Verfahren besteht darin, statt Funktionen $f \in \mathscr{L}\left(I\right)$ ihre Äquivalenzklassen $\left[f\right]$ in dem zugehörigen Quotientenvektorraum zu betrachten.»*
> > 
> 
> > [!requirements]-
> >  
> > *Seien:*
> > - *$I \subset \mathbb{R}$ ein Intervall, das:*
> > 	
> >     - *offen, halboffen oder abgeschlossen*
> >     - *beschränkt oder unbeschränkt​*
> > - *$\Sigma$ die $\sigma$-Algebra der Borelmengen auf $I$*
> > - *$\lambda$ das Lebesguemaß*
> > 
> 
> Sei ${L}^{p}$ der *«für ${} 1 \leq p\, \textless\, \infty$»* <u>zu dem auf $I$ definierten Lebesgue-Funktionenraum $\mathscr{L}^{p}$ zugehörige Quotientenraum</u>:
> 
> $$L^{p}\left(I\right):= \mathscr{L}^{p}\left(I\right)\,/\,\mathcal{N}_{p}$$
> 
> und wir definieren für ${} \left[f\right] \in {L}^{p}\left(I\right) {}$ die ***${L}^{p}$-Quotientennorm***: *«endlich kann das Sternchen verschwinden»*
> 
> $${\large\left\|{\normalsize\left[f\right]}\vphantom{sum}\right\|}_{p} := \left\|f\vphantom{A}\right\|_{p}^{\star} = \left(\int_{I}\left|f\right|^{p}\ \mathrm{d}\lambda\right)^{\frac{1}{p}}$$
> 
> *«Alternative Notation ist $\left\|\,{\cdot}\,\vphantom{A}\right\|_{{L}^{p}}$»*
> 
> Wir behaupten, dass $\left({L}^{p}\left(I\right)\ ,\,\left\|\,{\large\cdot}\,\vphantom{A}\right\|_{p}\right)$ ein ***Banachraum*** ist.
> 
> > [!hint]- Vereinfachter Umgang mit den Elementen des Quotientenraums $L^{p}$
> > 
> > Obwohl die **$L^{p}$-Räume eigentlich keine Räume von Funktionen, sondern von Äquivalenzklassen** von Funktionen sind, <u>behandelt man ihre Elemente, als wären es Funktionen.</u>
> > 
> > **Man schreibt also $f \in L^{p}$ statt $\left[f\right] \in L^{p}$ usw.** und ***in der Regel*** treten dadurch ***keine Komplikationen*** auf.
> > 
> > > [!attention]+ Mögliche Fallen bei der Behandlung der Äquivalenzklassen als Funktionen
> > > 
> > > Beispielsweise ist:
> > > 
> > > $$f\ \longmapsto \int_{I} f\ \mathrm{d}\lambda$$
> > > 
> > > eine <u>wohldefinierte Abbildung auf $L^{1}\left(I\right)$,</u> nicht jedoch:
> > > 
> > > $$f\ \longmapsto f\left(t_{0}\right)$$
> > > 
> > > denn ***für $g \neq \widehat{g}$ beide aus $\left[f\right]$ kann $g\left(t_{0}\right) \neq \widehat{g}\left(t_{0}\right)$ gelten*** und somit ist die <u>Abbildung der ganzen Äquivalenzklasse $\left[f\right]$ nicht wohldefiniert</u>.
> > > 
> > > ***
> > > 
> > > Ferner brauchen die ***Repräsentanten der $f \in L^{p}$ nur fast überall definiert*** zu sein; in diesem Simn ist etwa
> > > 
> > > $$t\ \longmapsto \frac{1}{\sqrt{t}}$$
> > > 
> > > ein <u>Element aus $L^{1}\left[0,1\right]$</u>.
> > > 
> 
> ###### `\start{proof}`
> 
> Alle nötigen Aussagen, also:
> 
> - dass der <u>Enttarnungsraum $\mathcal{N}_{p}$ ein Unterraum</u> von $\mathscr{L}^{p}\left(I\right)$ ist
> - die <u>Normeigenschaften</u> der Quotientennorm $L^{p}$
> - <u>Vollständigkeit</u> von $L^{p}$
> 
> folgen direkt aus dem [[Matematyka/Funktionalanalysis/Normierte Räume/Lebesgue-Räume#^e371d3\|Lemma I.1.9; Faktorisierung halbnormierter Räume durch den Nullraum]].
> 
> `\stop{proof}`
> 
>
{ #12ff64}

> 