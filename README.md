# utilisation de l'API
api réalisé en Node.JS
Pour lancer l'API, rendez-vous sur le chemin d'index.js, allumez un CMD et écrivez "node index.js"

# Composant_metier_agenda



## Description

Projet EPSI sur la réalisation d'une API en lien avec les diagrammes de classes et cas d'utilisations.


### Compte utilisateur
<br><br>
- Pour **se connecter** à un compte, il faut :
<br>
url : **/user/login**<br>
method : **POST**<br>
Content-Type : **application/json**<br>
data : JSON
{
    user : {
        email : <your_email>,
        password : <your_password>
    }
}
<br><br>
- Pour **se deconnecter** de son compte, il faut :
<br>
url : **/user/logout<br>
method : **POST**<br>
<br><br>
- Pour **renseigner un contacts** dans son agenda, il faut :
<br>
Content-Type : **application/json**<br>
data : JSON
{
    user : {
        numero : <numero>,
        nom : <nom>
        adresse : <adresse>
        email : <email>
        website : <website>
        apartenance_utilisateur : <utilisateur connecte>
    }
}
    <br><br>
  - Pour **supprimer un contact** dans son agenda, il faut :
<br>
  url : **/user/deleteuser<br>
method : **POST**<br>
Content-Type : **application/json**<br>
data : JSON
{
    user : {
        numero : <numero>,
        apartenance_utilisateur : <utilisateur connecte>
    }
}
    <br><br>
    - Pour **modifier un contact** dans son agenda, il faut :
<br>
    url : **/user/modifyuser<br>
method : **POST**<br>
Content-Type : **application/json**<br>
data : JSON
{
    user : {
        numero : <numero>,
        nom : <nom>
        adresse : <adresse>
        email : <email>
        website : <website>
        apartenance_utilisateur : <utilisateur connecte>
    }
}
    <br><br>
      - Pour **ajouter un contact** dans son agenda, il faut :
<br>
    url : **/user/adduser<br>
method : **POST**<br>
Content-Type : **application/json**<br>
data : JSON
{
    user : {
        numero : <numero>,
        nom : <nom>
        adresse : <adresse>
        email : <email>
        website : <website>
        apartenance_utilisateur : <utilisateur connecte>
    }
}
