# Projet-VR-Aquarium

Thoral Anaïs - Ré Simon

Réalité Virtuelle Aquarium



I/ Utilisation

Vous avancez automatiquement tout droit dans la scène. 
Pour tourner: Alt + mouvements de la souris

II/ Balade à l’infini et décors 

Pour ce qui est de la balade à l’infini nous avons fait une génération procédurale de terrain pour le sol de l’aquarium. Nous avons pu régler le dénivelé des courbes, les couleurs et nous avons mis en place en LOD. (voir dans Scripts/Terrain)

Nous avons aussi mis en place une génération procédurale pour les éléments de décors. (voir dans Scripts/Coral) Nous avons définit une surface autour du joueur où les coraux se généreront. Quand les coraux seront trop loin du joueur, ces derniers disparaîtront et nous en rajouterons des nouveaux. Tout est mis en place automatiquement. Leur place est aléatoire donc ils peuvent apparaître n’importe où autour du joueur. Nous pouvons choisir les coraux à faire apparaître dans l’éditeur sur Unity et le nombre maximum d’objet que nous voulons autour de nous. Ceci permet de se calibrer correctement pour chaque appareil. Le but étant que le jeu soit supportable pour la VR. 

III/ Gestion du brouillard de profondeur

Il s’agit d’un brouillard dit différé, qui est basé sur la texture de profondeur de la caméra. On va poser une couleur unie en faisant varier sa transparence sur les objets en fonction de leur distance à la caméra. Cela nous permet d’avoir un rendu qui ressemble à une vue sous-marine tout en nous permettant d’économiser des performances (les objets trop loin de la caméra ne sont pas rendus).

IV/ Gestion des poissons

Nous avons mis en place une génération procédurale de poissons. Ces dernier apparaissent autour du joueur à un rayon bien précis afin d’éviter qu’ils n’apparaissent pas comme par magie juste devant lui. Encore une fois lorsque le joueur s’éloigne trop d’un poisson celui-ci disparaît permettant à un autre d'apparaître près de lui. On peut, comme pour les coraux, choisir les poissons que nous voulons afficher, leur nombre, et plein d’autres paramètres qui nous permettent d’avoir un rendu plus fluide et réel. Nous avons ajouté aux poissons une animation pour que l’utilisateur ait l’impression que ces animaux nagent près de lui (voir dans Scripts/Fishes).
