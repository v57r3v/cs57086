java c
„Numerische Methoden II“
Wintersemester 2024/2025
Aufgabe 3 - PDE
Für das erfolgreiche Bestehen von Aufgabe 3 müssen lauffähige Programme, sowie ein kurzer Report zu den Aufgaben abgegeben werden.
Partielle Differentialgleichungen (PDE)
Bei einem Chemieunfall in Bad Cannstatt wurde der Neckar mit einem hochkonzentrierten Stoffgemisch auf Alkoholbasis verunreinigt. Um ein großes Fischsterben zu verhindern, muss die Kontamination entfernt werden. Dazu ist es nötig die örtliche Ausbreitung der Stoffe im Neckar abzuschätzen.

Betrachtet wird der Neckar. Es wird angenommen, dass der Transport der Schadstoffe im Neckar nur in x-Richtung stattfindet. D.h., dass sich die Konzentration der Schadstoffe über die Breite und die Tiefe im Flussbett nicht ändert. Das hierdurch vereinfachte Transportmodell ist in Abbildung b) dargestellt und kann durch die folgende eindimensionale Konvektions-Diffusions-Gleichung mit folgender Orts- und Zeitdimension beschrieben werden:

Hierin beschreibt uj(x,t) die Konzentration des Schadstoffes j, abhängig vom Ort x und der Zeit t. Es handelt sich somit um eine Partielle Differentialgleichung (PDE).
1. Teil:
Im ersten Teil dieser Aufgabe sind die effektiven Diffusionskoeffizienten Dj der Stoffe j und die Geschwindigkeit v über die Länge konstant und haben folgende Werte:
v = 0.2, D1 = 0.01, D2 = 0.005, D3 = 0.0005.
Am Start- und Endpunkt des Neckarabschnitts soll für die Zeitdauer der Berechnung ein zeitlich konstanter Konzentrationswert vorliegen, was einer Dirichlet-Randbedingung entspricht:
uj(x = 0,t) = 0,
uk(x = 1,t) = 0.
1. Um das Konzentrationsprofil des Stoffs j über x und t zu berechnen, muss die Transportgleichung diskretisiert werden. Leiten Sie hierfür die semidiskretisierte Form. im Ort mit dem Finite Volumen Verfahren (zentral Differenzen Schema und Upwind-Schema) für die Konvektions-Diffusions-Gleichung her.
2. Zum Zeitpunkt t = 0 findet der Chemieunfall statt, daher liegt als Anfangsbedingung der folgende Konzentrationsverlauf vor:

Erstellen Sie ein Programm, mit dem die semidiskretisierte PDE gelöst wird. Programmieren sie hierzu für die Diskretisierung der PDE das Finite Volumen Verfahren mit Zentraldifferenzen und das Upwind Verfahren. Für die örtliche Disktretisierung wird Δx = 0.02 und für die Integrationsschritteweite Δt = 0.01 angenommen.
Verwenden Sie zur L代 写Numerische Methoden II Wintersemester 2024/2025 Aufgabe 3 - PDEJava
代做程序编程语言ösung des ODE-Systems das Semi-implizite Euler Verfahren. Berechnen Sie in Ihrem Programm die numerische Péclet-Zahl.
3. Um die Genauigkeit der numerischen Lösung abschätzen zu können, wird ein Vergleich mit der analytischen Lösung für einen Konzentrationspuls in Form. eines Dirac-Pulses angestellt. Die Analytische Lösung der Konvektions-Diffusionsgleichung lautet für diesen speziellen Fall:

Vergleichen Sie die numerische Lösung der verschiedenen Diskretisierungsverfahren mit der analytischen Lösung, plotten Sie dafür die Konzentrationsprofile für t = { 0.5, 1.0} getrennt für den jeweiligen Stoff. Erklären Sie die Abweichung zur analytischen Lösung für beide Verfahren (und die Gründe dafür), und formulieren Sie eine Empfehlung, wie der Fehler verringert werden kann.
Nehmen Sie eine Integrationsschrittweite von Δt = 0.01 an. Für die örtliche Diskretisierung betrachten Sie Δx = {0.02, 0.01, 0.005}. Bestimmen Sie die numerische Péclet-Zahl. Wie verhält sich die numerische Péclet-Zahl sowie die Abweichung zur analytischen Lösung mit feinerer Diskretisierung?
2. Teil:
Im zweiten Teil dieser Aufgabe sind die effektiven Diffusionskoeffizienten Dj der Stoffe j konzentrationsabhängig und verändern sich damit auch über die Ortskoordinate. Für die Diffusionskoeffizienten gilt:

Es liegt wieder am Startpunkt des betrachteten Neckarabschnitts für die Zeitdauer der Berechnung ein zeitlich konstanter Konzentrationswert vor, was einer Dirichlet-Randbedingung entspricht:
uj(x = 0,t) = 0,
Am Ende des Abschnitts liegt nun ein konstanter Gradient der Konzentration vor, sog. Neumann-Randbedingung.

1. Leiten Sie hierfür unter Berücksichtigung der konzentrationsabhängigen Diffusionskoeffizienten die semidiskretisierte Form. der Konvektions-Diffusions-Gleichung her, und implementieren Sie sie in Ihrem Programm.
Hinweis:
 Als Bestandteil des Flussterms hängen die Diffusionskoeffizienten von den Zuständen auf den Rändern der Finite-Volumen-Zellen ab
2. Nach erfolgreicher Validierung des Modells sollen Sie nun abschätzen, zu welchem Zeitpunkt und Ortspunkt die maximale Konzentration des giftigen Stoffs C3 unter   u3 ≤ 1 sinkt?
Zum Zeitpunkt t = 0 findet der Chemieunfall statt, daher liegt als Anfangsbedingung der folgende Konzentrationsverlauf vor:

Hinweis:
 Plot max(uj) = f(t)



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
