# button-modal
En cliquant l'icône , il nous donne deux choix de liens différents :
- soit celle qui mène vers le linkedin de Tiavina 
-soit celle qui mène vers le lien du Linekdin de Sonia 

## étapes : 
1- Créer les fichiers : 
                        - index.php => *n'oublie pas d'ajouter les liens "link en css" et "script en js" 
                        - style.css
                        - main.js
                        
2- Ajoute l'icône de Linkedin en balise "img" dans l'html
      - Nommée: button
     
3- Ajoute un balise "div id"
      - Nommée: modale
      
 - Ajoute un autre "div class" 
      - Nomme-la: modal-content:
                             - ajoute un "span id" nommé close <span id="close" class="close">&times;</span> 
                             
                             - ajoute les liens avec la balise lien "a href"
                              
4- Type de style dans le css qu'on a choisi pour les boutons :
                          .modal {
                            display: none;
                            position: fixed;
                            z-index: 1; 
                            padding-top: 100px; 
                            left: 0;
                            top: 0;
                            width: 100%;
                            height: 100%;
                            overflow: auto;
                            background-color: rgb(0,0,0);
                            background-color: rgba(0,0,0,0.4); 
                          }

                          .modal-content {
                              background-color: #fefefe;
                              margin: auto;
                              padding: 20px;
                              border: 1px solid #888;
                              width: 80%;
                          }

                          .close {
                              color: #aaaaaa;
                              float: right;
                              font-size: 28px;
                              font-weight: bold;
                          }

                          .close:hover,
                          .close:focus {
                              color: #000;
                              text-decoration: none;
                              cursor: pointer;
                          }   

5- On a utilisé "const" pour appeller les "id".
    - Pour les fonctions , on les a écrit: 

                          button.addEventListener("click",function(){
                              modal.style.display="block";
                          })

                          close.addEventListener("click",function(){
                              modal.style.display="none";
                          })

                              

