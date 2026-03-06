"# Exercice 1" 
for (int j = 1; j<=jours; j++){
        achats = rand()%15+1;
        if ( achats > stock){
            achats = stock;
        }
        stock -= achats;
        if(stock<SeuilCommande &&commande ==0){
            commande = 50;
    }
    if (commande>0){
        stock += commande;
        commande = 0;
        cout<<"Jour" <<j <<"|stock : " <<stock <<"|Achats : " <<achats <<endl;
        if (stock<SeuilAlerte){
            cout<<"Alerte : Stock faible ! " <<endl;
        }