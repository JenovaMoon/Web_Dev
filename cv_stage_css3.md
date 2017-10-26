<!DOCTYPE HTML>
<html>

<head>
    <meta charset="utf-8" />
    <link href="https://fonts.googleapis.com/css?family=Cinzel:400,700" rel="stylesheet">
    <link rel="stylesheet" href="../cv_stage_css/style.css"/>
    <title>CV Prénom Nom</title>
</head>

<body>

    <div id="bloc_page">

        <div id="conteneur">
            <header>
                <p><img class="img" src="img/carte_visite.jpg" alt="" title="Coordonnées Prénom Nom"/></p>
                <h1>Prénom Nom</h1>  
            </header>

            <div id="objet"><h1>Candidature spontanée à un stage d'immersion</h1></div>


            <section id="CV">
                <div class="cv">
                    <h2>Mon expérience</h2>
                    <ul>
                        <li><strong>01/2014 - 12/2015 : ********</strong> : Agent de courrier</li>
                        <li><strong>08/2010 - 05/2011 : ********</strong> : Agent de courrier/Hôtesse d'accueil</a></li>
                        <li><strong>02/2002 - 10/2002 : ********</strong> : Agent d'administratif</li>
                        <li><strong>01/2002 - 12/2007 : Interim</strong> : Agent d'administratif/Hôtesse d'accueil/Manutention</li>
                        
                    </ul>
                </div>

                <div class="cv">
                    <h2>Ma Formation</h2>
                    <ul>
                        <li><strong>2016 à ce jour : Formation Développeur Web Junior</strong> - OpenClassrooms</li>
                        <li><strong>2012 : Formation en langue Anglaise TOEIC (Obtenu : 830)</strong> - Formalangue Paris</li>
                        <li><strong>2004 : LICENCE LLCE Italien (Niveau)</strong> - Sorbonne Nouvelle Paris III</li>
                        <li><strong>2003 : DEUG LLCE Italien (Obtenu)</strong> - Sorbonne Nouvelle Paris III</a></li>
                        <li><strong>2001 : Baccalauréat Générale Session Littéraire (Obtenu)</strong> - Lycée Mozart</li>
                        
                    </ul>
                </div>
            </section> <!-- Fin section cv-->


            <section id="autres">
                <div class="competences">
                    <h2>Mes compétences</h2>
                    <ul><strong>Générale</strong>
                        <li>Organisée, Rigoureuse, Adaptation</li>
                        <li>World / Excel</li>
                    </ul>

                    <ul><strong>Développement</strong>
                        <li>HTML5 / CSS3</li>
                        <li>BootStrap</li>
                        <li>WorldPress</li>
                        <li>PhP 7 / PhP Admin / MySQL</li>
                        <li>JavaScript (base)</li>
                        <li>Git & GitHub (base)</li>
                    </ul>

                    <ul><strong>Langues</strong>
                        <li><strong>Anglais</strong> : Correct</li>
                        <li><strong>Italien</strong> : Courant</li>
                    </ul>
                </div>

                <div class="loisirs">
                    <h2>Mes Loisirs</h2>
                    <ul>
                        <li>Jeu Video</li>
                        <li>Nail'Art</li>
                        <li>Lecture</li>
                        <li>Série</li>
                        <li>Nature</li>
                    </ul>
                </div>
            </section> <!--Fin section autres-->

        </div> <!--conteneur-->
    </div> <!--bloc_page-->
</body>
</html>


````
/* Définition des polices personnalisées */

@font-face {
    font-family: 'milkshakeregular';
    src: url('font/milkshake.eot');
    src: url('font/milkshake.eot?#iefix') format('embedded-opentype'),
         url('font/milkshake.woff') format('woff'),
         url('font/milkshake.ttf') format('truetype'),
         url('font/milkshake.svg#milkshakeregular') format('svg');
    font-weight: normal;
    font-style: normal;

}

/* Paramètre de la page */

body {
    font-family: 'Cinzel', serif;
    background: url('img/green_bg.jpg') fixed no-repeat;
    color:rgb(255, 255, 255);
}

#bloc_page {
	display: flex;
    width: 95%;
    justify-content: space-between;	
}

#conteneur
{
	width: 90%;
}

#objet {
    text-align: center;
    margin-top: 70px;
}


/* Header */
header, h1 {
    font-family: 'milkshakeregular', Arial, Verdana, serif;
    font-size: 2.2em;
    text-align: center;
    margin-bottom: -30px;
    
}

.img
{
	float: left;
	border: ridge rgb(56,102,3);
	box-shadow: 5px 5px 0px rgb(228,243,178)
}


/* section */
section {
    display: flex;
    margin-left: px;

}

#CV {
    padding-top: 125px;
    margin-left: 0px;
}

#autres {
    margin-left: 365px;
}

.loisirs {
    margin-left: 190px;
}
````
