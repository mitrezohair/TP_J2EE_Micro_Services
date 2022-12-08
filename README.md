# TP_J2EE_Micro_Services
- Première partie : (Customer-Service, Inventory-Service, Spring Cloud Gateway, Eureka Discovery) - 
- Deuxième Partie : Billing Service avec Open Feign Rest Client
- Troisième Partie :      Créer un Client Angular, 

Créer une application basée sur une architecture micro-service qui permet de gérer les factures contenant des produits et appartenant à un client.

Travail à faire :


1.Créer le micro-service customer-service qui permet de gérer les client

![Service_Customer_Service](https://user-images.githubusercontent.com/74791123/206469138-e046e9cd-7ca8-4374-a34d-26f2251ef9a7.PNG)

2.Créer le micro-service inventory-service qui permet de gérer les produits

![Service_Inventory_Service](https://user-images.githubusercontent.com/74791123/206469581-41b923b1-6a4b-4b65-9d68-db1e12731e71.PNG)

3. Créer la Gateway Spring cloud Gateway avec une Configuration statique du système de routage
      ==>Extrait de code qui montre la Configuration statique
      
      ![Code_Service_Gateway](https://user-images.githubusercontent.com/74791123/206472850-9347d7ec-42eb-44c4-a24c-b02ff65ddb4b.PNG)
      
      ==>Capture d'ecran qui montre l'execution de la Gateway (voir URL)
                                **** Inventory Service ****
                                
      ![Gateway_Service_Products](https://user-images.githubusercontent.com/74791123/206473722-8399293e-fa89-4949-95e8-db8827e881bf.PNG)
      
                                **** Customer Service ****
                                
      ![Gateway_Service_Customers](https://user-images.githubusercontent.com/74791123/206474730-551c1175-f0ce-4fab-a723-6b8e4a29c92f.PNG)

4. Créer l'annuaire Eureka Discrovery Service

![Spring_Eureka](https://user-images.githubusercontent.com/74791123/206470101-48dd7129-50dc-4be3-ad36-c8fd0d331e46.PNG)

5. Faire une configuration dynamique des routes de la gateway
        ==>Extrait de code qui montre la Configuration dynamique
        
        ![Gateway_Dynamic](https://user-images.githubusercontent.com/74791123/206475672-b1dc04f3-c51b-4a3d-a82e-ad4d1446d628.PNG)

        ==>Capture d'ecran qui montre l'execution de la Gateway Dynamiquement (voir URL)
                                        **** Inventory Service ****
                                        
        ![Inventory_Dynamique_Gateway](https://user-images.githubusercontent.com/74791123/206476469-08c751ca-7d03-46f8-9a9b-ffc589c85d80.PNG)

                                        **** Customers Service ****
                                        
        ![Customers_Dynamique_Gateway](https://user-images.githubusercontent.com/74791123/206477053-a08feaab-4e98-433e-8a90-f665a3b3320f.PNG)

6. Créer le service de facturation Billing-Service en utilisant Open Feign

7. Créer un client Web Angular (Clients, Produits, Factures)

8. Déployer le serveur keycloak :
     - Créer un Realm
     - Créer un client à sécuriser
     - Créer des utilisateurs
     - Créer des rôles
     - Affecter les rôles aux utilisateurs
     - Tester les différents modes d'authentification avec Postman en montrant les contenus de Access-Token, Refresh Token 
9. Sécuriser les micro-services et le frontend angular en déployant les adaptateurs Keycloak

10. Ajouter des Fonctionnalités supplémentaires de votre choix
