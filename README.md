# Bachelorarbeit-Quantensimulation

Dieses repository enthält sämtliche jupyter-Notebooks, die im Rahmen meiner Bachelorarbeit erstellt wurden.

## Installation

Um die Notebooks auszuführen, müssen Qiskit, Python und numpy installiert sein. Für einige Visualisierungen ist auch eine matplotlib und scipy Installation nötig.

## Benutzung

Es folgt eine kurze Beschreibung der Simulationen, die die entsprechenden Notebooks ausführen.

 - **qft.ipynb**: Enthält die Funktionen zur Durchführung einer Quanten-Fouriertransformation und einer inversen Quanten-Fouriertransformation, sowie ein Beispiel, um die Funktionen zu testen 
*Bemerkung: Die Funktionen führen die QFT, bzw. iQFT auf allen Qubits des übergebenen circuits aus. Um die QFT nur auf einer bestimmten Anzahl von Qubits n durchzuführen, muss n als zusätzliche Variable übergeben werden und darf nicht in der Funktion "qft" aus dem circuit bestimmt werden*
- **qs_delta.ipynb**: Simuliert die Zeitentwicklung einer Delta-Funktion mit dem QASMSimulator
- **qs_gauss.ipynb**: Simuliert die Zeitentwicklung einer Gauß-Kurve mit dem QASMSimulator
- **qs_gauss_impuls.ipynb**: Simuliert die Zeitentwicklung einer Gauß-Kurve mit Anfangsimpuls mit dem QASMSimulator und dem StatevectorSimulator



 Für alle folgenden Simulationen wird der StatevectorSimulator genutzt
- **qs_direkte_berechnung.ipynb**: Simuliert die Zeitentwicklung einer Gauß-Kurve mit Anfangsimpuls mit dem StatevectorSimulator. Für die Faktorisierung des Zeitentwicklungsoperators wurde die Phasenverschiebung durch den Impulsoperator direkt berechnet.
- **qs_interferenz.ipynb**: Simuliert die Zeitentwicklung zweier Gaußscher Wellenpakete, die miteinander interferieren
- **qs_potentialstufe.ipynb**: Simuliert die Zeitentwicklung eines Gaußschen Wellenpaketes mit einer Potentialstufe
- **qs_potentialtopf.ipynb**: Simuliert die Zeitentwicklung verschiedener Eigenzustände und eines Überlagerungszustandes in einem Potentialtopf
- **qs_tunneleffekt.ipynb**: Simuliert die Zeitentwicklung eines Gaußschen Wellenpaketes mit einem Potentialwall
- **qs_harmonischer_oszillator.ipynb**: Simuliert die Zeitentwicklung einer Delta-Funktion/Gauß-Kurve in einem quadratischen Potential


Bei der Initialisierung des Anfangszustandes ist darauf zu achten, dass die vollständige Wellenfunktion auf dem Ortsgitter abgebildet wird und nicht Teile über das Intervall hinausgehen. Dies würde zu verfälschten Simulationsergebnissen führen.
