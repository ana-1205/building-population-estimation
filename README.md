# Maturaarbeit im Fach Informatik

Thema: KI gestützte Gebäudeerkennung und Bevölkerungsschätzung mit Maks-R-CNN  

 Abstract:  
In dieser Maturaarbeit wird die Anwendung von künstlicher Intelligenz zur automatischen Gebäudeerkennung und darauf aufbauenden Bevölkerungsschätzung untersucht. Basierend auf dem Mask-R-CNN Modell für Instanzsegmentierung wurde ein eigenes Modell entwickelt, das Gebäude in Orthofotos der Schweiz erkennt und deren Grundflächen berechnet. Das Modell erreichte eine Präzision von 0.83 und einen Recall von 0.89, was auf eine hohe Trefferquote bei gleichzeitig geringer Fehlklassifikation hindeutet. Die anschliessende Bevölkerungsschätzung basiert auf gemeindespezifischen Dichtefaktoren. Die Validierung in drei Testgemeinden ergab Abweichungen von - 30% bis + 30% gegenüber den offiziellen Einwohnerzahlen von Ende 2021. Diese Arbeit zeigt somit die potentielle Eignung des Ansatzes, erkennt jedoch auch Limitationen bei dichter Bebauung. Dies schränkt den aktuellen Einsatz auf grobe Schätzungen ein.  Für zukünftige Forschungen können zusätzliche Datenquellen wie Gebäudehöhen integriert werden. Auch würde die Verfeinerung der Dichtefaktoren sowie der Einsatz von Transfer-Learning auf andere Regionen das Modell verbessern. Durch diese Ansätze könnte die Genauigkeit weiter gesteigert werden und das Modell für präzisere Bevölkerungsvorhersagen genutzt werden.   

## Quellenangabe und Code-Attribution

### Externe Quellen und Grundlagen
Basis: https://christianjmills.com/posts/pytorch-train-mask-rcnn-tutorial/

**Preparation**   
- important dependencies (= "Setting Up Your Python Enviroment", "Importing the Rquired Dependencies")  
- Project setup (= "Settin Up the Project")  
*Anpassungen*: Pfade angepasst
- Loading dataset (= "Loading and Exploring the Dataset")  
  *Anpassungen*: Pfade angepasst
- Image Annotation (= "Inspecting the Class Distribution", "Ptreparing the Data")   
 image classes, labels/ background class, visualisation annotations, segmentation polygons to images  
*Anpassungen*: split into training, validation and test (Hinzufügen von Testdatensatz)

**Mask R CNN**  
- initialising + summary (= Loading the Mask R-CNN Model)  
- data augmentation (= Data Augmentation)
  - image size (= Set training image size)
  - transforms (= Initialize the transforms)
- Building Dataset
  - image transforms (= Image Transforms)
  - initialising Dataset (= Initialise Datasets)
- colour map (= Save the Color Map)
- training parameters (= Configure the Training Parameters)

### Mit KI überarbeitet
- Building dataset
- Training Loop
- Train model

### Vollständig KI-generierte Komponenten
Die restlichen Code-Komponenten, die hier nicht aufgezählt wurden, wurden vollständig mit ChatGPT oder DeepSeek erstellt und für die spezifischen Anforderungen der Gebäudeerkennung adaptiert.
