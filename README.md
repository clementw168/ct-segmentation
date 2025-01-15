# ct-segmentation

This is a simple project to visualize the segmentation of 3D pulmonary CT images.


## Tasks lists

- [x] Import the data and visualize the images
- [] Compute segmentation and visualize the results
  - [] Implement Frangi filter
  - [] Implement Sato filter
  - [] Implement a simple thresholding algorithm
- [] Compute metrics to evaluate the segmentation
- [] Compare the results: metrics and visualizations
- [] Create a simple Streamlit app to visualize the results


vol_01.nii.gz : Volume CT 3D
lungs_01.nii.gz : Segmentation 3D des poumons
vessels_01.nii.gz : Segmentation 3D de référence des vaisseaux du poumon (pour validation)
L’objectif du mini-projet est de générer une segmentation des vaisseaux du poumon à partir du volume CT et de la segmentation des poumons. Le candidat devra écrire un code en python pour réaliser les tâches suivantes :

Calculer les cartes de Vesselness sur le volume du poumon (Frangi, Sato, ou autre).
Comparer les performances des filtres de vesselness avec une technique simple de seuillage direct des intensités du volume CT à l’intérieur du masque des poumons
Comparer les différentes méthodes avec une courbe ROC. Quelle est la meilleure méthode et pourquoi ? 
Quel est le meilleur seuil pour les différentes cartes ?
TIPS :

Vous pouvez utiliser Slicer3D pour la visualisation de données.
Utilisez de préférence les packages suivants : skimage, sklearn, simpleITK
Lors de la restitution, nous te proposons l’ordre suivant :

Explication des méthodes utilisées (10 min)
Explication du code avec une demo en live sur certains cas de la base de données (10 min)
Explication des résultats (10 min)
Discussion
La restitution sera suivie d’un entretien technique avec les ingénieurs de l’équipe.