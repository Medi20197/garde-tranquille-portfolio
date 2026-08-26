# Garde Tranquille — documentation fonctionnelle publique

- **Étude de cas :** https://medi20197.github.io/garde-tranquille-portfolio/#top
- **Démonstration interactive :** https://medi20197.github.io/garde-tranquille-portfolio/demo.html
- **Dépôt public :** https://github.com/Medi20197/garde-tranquille-portfolio

Cette page décrit les capacités fonctionnelles observables de l’application. Les règles de calcul, données, identités, configurations et structures internes restent privées.

## Fonctionnalités de l’application

### Authentification et contrôle d’accès

- connexion sécurisée à l’application ;
- distinction entre profil administrateur et profil standard ;
- tableau de bord et rapports réservés aux profils autorisés ;
- navigation adaptée aux droits de l’utilisateur ;
- contrôle du compte actif.

### Gestion multisite

- sélection du site actif depuis l’interface ;
- isolation et rechargement des données selon le site sélectionné ;
- administration des sites pour les profils autorisés.

### Tableau de bord

- indicateurs synthétiques sur le personnel, les permanences et les absences ;
- aperçu des prochaines permanences ;
- accès rapide aux principaux modules ;
- notifications liées aux congés.

### Personnel

- liste, recherche, filtres et pagination ;
- création, consultation, modification et suppression d’un profil ;
- gestion du statut, de la fonction et de l’affectation ;
- affectations temporelles, permutations et intérims ;
- consultation de l’historique des affectations ;
- import de personnel depuis Excel, XLS ou CSV.

### Planning des permanences

- navigation mensuelle ;
- génération d’une proposition de planning ;
- ajout, modification, déplacement et suppression d’une permanence ;
- prise en compte des absences, jours fériés et exemptions sans exposer les règles de calcul ;
- signalement des anomalies avant validation ;
- validation et changement d’état du planning ;
- conservation et consultation des révisions ;
- export d’un mois ou d’une période en PDF et Excel.

### Shifts opérationnels

- génération pour une journée, une période ou un mois ;
- affichage calendrier et affichage détaillé par groupe ;
- filtrage par cellule et tri par groupe ou créneau ;
- modification des horaires et groupes ;
- ajout, retrait et permutation d’affectations ;
- détection visuelle des anomalies ;
- sauvegarde et validation ;
- export PDF et Excel.

### Absences, congés et exemptions

- création, modification et suppression d’une absence ;
- suivi annuel des congés et de leur incidence sur le planning ;
- notifications de départ et de retour ;
- création, modification, clôture et suppression d’exemptions ;
- exemptions temporaires ou permanentes ;
- régénération du planning après modification.

### Rapports et traçabilité

- statistiques de charge par personne et par type de permanence ;
- sélection du mois analysé ;
- historique des autorisations avec filtres ;
- exports PDF et Excel du planning et des autorisations ;
- journal d’audit des actions ;
- pagination des historiques.

### Expérience utilisateur

- interface responsive ;
- barre latérale repliable ;
- écrans d’erreur et page 404 ;
- synchronisation des données lors du retour sur l’application.

## Fonctionnalités de la démonstration publique

La page `demo.html` reproduit uniquement une version fictive et simplifiée :

- tableau de bord avec indicateurs et prochaines permanences ;
- personnel fictif avec recherche et filtres ;
- calendrier mensuel avec ajout, déplacement, génération, validation et réinitialisation locales ;
- absences et exemptions fictives ;
- services opérationnels avec filtre et génération simulée ;
- rapports et historique simulés ;
- boutons d’export simulés, sans création de fichier réel.

Les modifications de la démonstration restent dans la page courante et disparaissent au rechargement. Elle ne possède ni authentification réelle, ni backend, ni base de données.

## Écarts assumés entre l’application et la démonstration

| Capacité | Application | Démonstration publique |
|---|---:|---:|
| Authentification et rôles | Oui | Simulés visuellement |
| Backend et persistance | Oui | Non |
| Multisite | Oui | Sélecteur fictif |
| Gestion complète du personnel | Oui | Recherche et filtres locaux |
| Génération métier des plannings | Oui | Logique simplifiée |
| Révisions et audit persistants | Oui | Affichage simulé |
| Exports PDF et Excel | Oui | Boutons simulés |
| Données réelles | Privées | Aucune |

## Publication GitHub Pages

La vitrine est publiée depuis `main`, dossier `/ (root)`, avec **Deploy from a branch**. `index.html` contient l’étude de cas et `demo.html` la démonstration.

```bash
git add .
git commit -m "Mettre à jour la vitrine Garde Tranquille"
git push
```

[Index des trois projets](https://github.com/Medi20197/mailflow-demo/blob/main/GITHUB_PAGES.md)
