# Composant_metier_agenda



## Description

Projet EPSI sur la réalisation d'une API en lien avec les diagrammes de classes et cas d'utilisations.


### Compte utilisateur
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
