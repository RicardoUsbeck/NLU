# Natural Language Understanding
## Vorlesung 3: "Algorithmen zur Bestimmung der Levenshtein-Distanz von Zeichenketten"

In dieser Vorlesung gehen wir auf verschiedene Algorithmen zur Berechnung der Levenshtein-Distanz zwischen zwei Strings ein. Dabei lernen wir drei verschiedene Algorithmen zur Berechnung kennen.

Das Colab-Jupyter-Notebook finden Sie unter https://colab.research.google.com/drive/1kZ7BP9OZ9Z2WSTcJrGGKcBpNLBXfWErt#scrollTo=gN78e6up20he&line=1&uniqifier=1 oder als Datei in diesem Repository.

### Selbsttestfragen
* Schreiben Sie einen korrekten Algorithmus für die Hamming-Distanz (siehe Quellen)!
* Beweisen Sie dass, editDistanz <= hammingditanz?
* Geben Sie für zwei String unterschiedlicher Länge den Upper und Lower Bound für die Edit-Distanz an!
* Bauen Sie den Code so um, dass bei der rekursiven Variante die Anzahl der Calls mitgeloggt und auf der Kommandaozeile geschrieben wird!
* Wenn man die Kosten für replace unendlich groß macht, löst man das longest common subsequence problem. Beweise Sie!
* Wie hoch sind die Levenshtein-Kosten, die cat in catcat verwandeln?
* Wenn wir nur an dem Abstand interessiert sind, wenn er kleiner als ein Schwellenwert k ist, dann genügt es, einen diagonalen Streifen der Breite 2k+1 in der Matrix zu berechnen. Auf diese Weise kann der Algorithmus in O(kl)-Zeit ausgeführt werden, wobei l die Länge des kürzesten Streifens ist. Beweisen Sie!
* Durch Untersuchung von Diagonalen anstelle von Zeilen und durch Verwendung einer faulen Auswertung, können wir die Levenshtein-Distanz in O(m (1 + d)) Zeit finden (wobei d die Levenshtein-Distanz ist), die viel schneller als der reguläre Algorithmus zur dynamischen Programmierung ist, wenn die Distanz klein ist. Beweisen Sie!
* Wir können unterschiedliche Kosten für das Einfügen, Löschen und Ersetzen festlegen. Wir können auch Strafkosten angeben, die davon abhängen, welche Zeichen eingefügt, gelöscht oder ersetzt werden. Bei welchen Szenarien macht das Sinn?
* Dieser Algorithmus parallelisiert schlecht, aufgrund einer großen Anzahl von Datenabhängigkeiten. Was kann man parallelisieren?

### Quellen
* Cormen, T. H., Leiserson, C. E., Rivest, R., and Stein, C. (2017). Algorithmen-Eine Einführung. Walter de Gruyter GmbH and Co KG.
* Jurasky, D., and Martin, J. H. (2000). Speech and Language Processing: An introduction to natural language Processing. Computational Linguistics and Speech Recognition. Prentice Hall, New Jersey. (https://web.stanford.edu/~jurafsky/slp3/2.pdf)
* Levenshtein, V. I. (1966, February). Binary codes capable of correcting deletions, insertions, and reversals. In Soviet physics doklady (Vol. 10, No. 8, pp. 707-710).
* Wagner, R. A., and Fischer, M. J. (1974). The string-to-string correction problem. Journal of the ACM (JACM), 21(1), 168-173. (https://dl.acm.org/doi/pdf/10.1145/321796.321811)
* Fred J. Damerau: A technique for computer detection and correction of spelling errors. In: Communications of the ACM. Band 7, Nr. 3, März 1964, S. 171–176.
* http://www.let.rug.nl/kleiweg/lev/, 24.06.2020, Online Tool
* https://en.wikibooks.org/wiki/Algorithm_Implementation/Strings/Levenshtein_distance\#Python, 21.06.2020 


### Lernvideos/Blended Learning
* https://www.youtube.com/watch?v=HXNhEYqFo0o, 14.06.2020
* https://www.youtube.com/watch?v=MiqoA-yF-0M, 19.06.2020 
* https://www.youtube.com/watch?v=OQ5jsbhAv_M, 19.06.2020
* https://www.youtube.com/watch?v=Xxx0b7djCrs, 19.06.2020
* https://www.youtube.com/watch?v=ocZMDMZwhCY, 19.06.2020
* https://www.youtube.com/watch?v=8Q2IEIY2pDU, 21.06.2020
* https://www.youtube.com/watch?v=qp8YwtvS3Uo, 21.06.2020
* https://www.youtube.com/watch?v=xFd5P9nyhTw, 30.06.2020
