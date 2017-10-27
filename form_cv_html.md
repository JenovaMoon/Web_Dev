````
<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8"/>
    <link rel="stylesheet" href=""/>
    <title>Formulaire Cv</title>
</head>

<body>
    <form method="post" action=""> <!-- nom du fichier PHP à préciser -->
        <fieldset> <!-- Partie état civil -->
            <legend>Etat civil</legend> <!-- Titre du champ (fieldset) -->

            <p><label for="nom">Nom</label>
            <input type="text" name="nom" id="nom" required autofocus /></p>

            <p><label for="prenom">Prénom</label>
            <input type="text" name="prenom" id="prenom" required /></p> 

            <p><label for="date_naissance">Date de naissance</label>
            <input type="date" name="date_naissance" id="date_naissance" required /></p>
        </fieldset>

        <fieldset> <!-- Partie coordonnées -->
            <legend>Vos coordonnées</legend> 

            <p><label for="adresse">Votre adresse</label>
            <input type="text" name="adresse" id="adresse" required /></p>

            <p><label for="tel">Votre n° de téléphone</label>
            <input type="tel" name="tel" id="tel" required /></p>

            <p><label for="email">Votre email</label>
            <input type="email" name="email" id="email" required /></p>

            <p><label for="site">votre site</label>
            <input type="url" name="site" id="site"/></p>
        </fieldset>

        <fieldset> <!-- Partie formation -->
            <legend>Vos formations</legend> 

            <p><label for="diplome">Diplôme Obtenu</label>
            <input type="text" name="diplome" id="diplome"/></p>

            <p><label for="annee_diplome">Date d'obtention du diplôme</label>
            <input type="date" name="annee_diplome" id="annee_diplome"/></p>

            <p><label for="lieu">Etablissement d'obtention du diplôme</label>
            <input type="text" name="lieu" id="lieu"/></p>
        </fieldset>

        <fieldset> <!-- Partie expérience -->
            <legend>Vos expériences</legend> 

            <p><label for="annee">Année</label>
            <input type="date" name="annee" id="annee" required /></p>

            <p><label for="societe">Nom de la société</label>
            <input type="text" name="societe" id="societe" required /></p>

            <p><label for="job">Intitulé du poste</label>
            <input type="text" name="job" id="job" required /></p>

            <p><label for="descriptif">Description du poste</label>
            <textarea name="descriptif" id="descriptif" row="10" cols="50" required></textarea></p>          
        </fieldset>

        <fieldset> <!-- Partie compétences -->
            <legend>Vos compétences</legend> 

            <p><label for="lang">Langues</label>
            <input type="text" name="lang" id="lang"></p>

            <p><label for="informatique">Informatique</label>
            <input type="text" name="informatique" id="informatique"/></p>

            <p><label for="lang_info">Langage Informatique</label>
            <input type="text" name="lang_info" id="lang_info"/></p>

            <p><label for="autres">Autres</label>
            <textarea name="autres" id="autres" row="10" cols="50"></textarea></p>          
        </fieldset>

        <fieldset> 
            <legend>Centres d'intérêts</legend>

            <p><label for="loisirs">Quels sont vos loisirs ou vos divers centres d'intérêts?</label> <br/>
            <textarea name="loisirs" id="loisirs" rows="10" cols="50"></textarea></p>
        </fieldset>

        <input type="submit" value="Envoyer" />
    </form>

</body>
</html>
````
