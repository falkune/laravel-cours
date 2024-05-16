Table "Utilisateurs" :
    ID_Utilisateur (Clé primaire)
    Nom
    Prénom
    Email
    Mot de passe

Table "Hebergements" :
    ID_Hebergement (Clé primaire)
    ID_Utilisateur (Clé étrangère faisant référence à la table Utilisateurs)
    Titre
    Localisation
    Description
    Images

Table "Reservations" :
    ID_Reservation (Clé primaire)
    ID_Hebergement (Clé étrangère faisant référence à la table Hebergements)
    Date_Debut
    Date_Fin
    ID_Heberge (Clé étrangère faisant référence à la table Utilisateurs, pour l'utilisateur qui effectue la réservation)