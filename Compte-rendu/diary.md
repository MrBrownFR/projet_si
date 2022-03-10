# Compte-rendu du projet de SI

- **[DATE]** : [Texte] (+ photos)
- **03/03** : Après analyse du système actuel, la [réutilisation de la carte NXT](../TermSIArcheo2022) pour le contrôle des moteurs semble être la meilleure solution. Une manette est aussi utilisée pour l'interface utilisateur. Le câblage des moteurs est pour l'instant temporaire.
- **07/03** : Les moteurs ont été étiquetés et référencés afin de faciliter la coordination entre programmation et conception. CODAGE DES MOTEURS : 
  - Resserer / deserrer la pince :
    - Port A
    - Contrôle : gâchettes
  - Monter / descendre la pince :
    - Port B
    - Contrôles : joystick droit
  - Roues : 
    - Port 1
    - Contrôle : joystick gauche
- **08/03** : Après concertation avec l'équipe en charge de l'ingénérie, la répartition des moteurs a évolué comme suit : 
  - ```mermaid
    graph TD
    A(Contrôle des roues) --> B(Port 1 : Relais moteur)
    B(Port 1 : Relais moteur) --> C(Roue gauche : Motor 1)
    B(Port 1 : Relais moteur) --> D(Roue droite : Motor 2)
    E(Monter / Descendre la pince) --> F(Port 2 : Relais moteur)
    F(Port 2 : Relais moteur) --> G(Servomoteur : Motor 1)
    H(Resserer / desserer la pince) --> I(En attente de Tristan)
    ```
  - La programmation globale du robot est terminé, je suis en train de préparer les câbles nécessaires, ranger les moteurs et commencer à assembler les différents "modules" ensembles. La batterie qui contrôle le robot a son fusible mort, les tests sont donc pour l'instant impossibles car le boîtier NXT est incapable d'alimenter les servomoteurs non-LEGO.
