Partie 2 / Membre 3 => groupe 3

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inscription DevConf 2025</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>DevConf 2025 - Inscription</h1>
        <p>Compte à rebours : <span id="countdown">00:00:00</span></p>
    </header>
    <div class="left">
    <form id="registrationForm">
        <div class="name">
        <label for="name">Nom : <input type="text" id="name" required></label>
        
        <label for="username">Prénom : <input type="text" id="name" required></label>

        <label for="email">Email : <input type="email" id="email" required></label>
        </div>

        <h2>Type de billet : </h2>
        <div class="input">
            <label>
                Standard
                <input type="radio" name="ticket" value="standard">
            </label>

            <label>
                VIP
                <input type="radio" name="ticket" value="vip">
            </label>

            <label>
                Etudiant
                <input type="radio" name="ticket" value="etudiant">
            </label>
        </div>
        <div class="atelier">
        <h2>Ateliers (cases à cocher) :</h2>
        <label>
            Développeur web 
            <input type="checkbox" name="workshop" value="web">
        </label>
        <label>
            Développeur Mobile
            <input type="checkbox" name="workshop" value="mobile">
        </label>
        </div>

        <div class="repas">
        <h2>Options repas :</h2>
        <label>
            Végétarien
            <input type="checkbox" name="meal" value="vegetarien"> 
        </label>

        <label>
            Sans gluten
            <input type="checkbox" name="meal" value="sans-gluten"> 
        </label>
        </div>
        <button type="submit">S'inscrire</button>
    </form>
    </div>

    <div class="right">
    <section id="programme">
        <h2>Programme</h2>
        <table>
            <tr><th>Horaire</th><th>Session</th></tr>
            <tr><td>09:00</td><td>Keynote</td></tr>
        </table>
    </section>

    <section id="intervenants">
        <h2>Intervenants</h2>
        <div class="intervenants">
            <h3>Photo </h3>
            <h3>Nom </h3>
            <h3>Sujet </h3>
        </div>
        <div class="images-nom">
            <img src="4983d1d7-d9ff-4773-8696-97f735e90031.jpeg" alt="">
            <img src="5aac4b1809430d6c8e49a6a98e95ffc9.jpg" alt="">
            <img src="56a150617b64ea9840b1cb78170ace4b.jpg" alt="">
        </div>
        <div class="nom">
            <p>James BLOND</p>
            <p>Seo-ARI</p>
            <P>Arial Stark</P>
        </div>
    </section>
    </div>
</body>
</html>





body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #ccc;
    overflow-x: hidden;
    overflow-y: auto;
    height: 90vh;
}
.left{
    width: 45%;
    background-color:transparent;
    border-radius: 30px;
    left: 20px;
    position: relative;
    border: 2px solid #814700;
    top: 20px;
}
.right{
    width: 50%;
    height: 770px;
    background-color:transparent;
    border-radius: 30px;
    left: 750px;
    position: relative;
    border: 2px solid #814700;
    bottom: 750px;

}
h2{
    text-decoration: underline;
}
.name label .atelier label .repas label{
    display: block;
}

.repas input{
    display: block;
    top: -20px;
    position: relative;
    left: 10px;
}
.atelier input{
    display: block;
    top: -20px;
    position: relative;
    left: 10px;
    
}
.name input{
    display: block;
    top: -30px;
    position: relative;
    left: 70px;
}
header {
    background: #814700;
    color: white;
    text-align: center;
    padding: 20px;
}


form {
    margin: 20px;
    display: flex;
    flex-direction: column;
}

input {
    margin: 5px 0;
    padding: 8px;
    border: 2px solid #ccc;
    width: 50%;
    outline: none;
}
.email{
    left: 70px;
    position: relative;
}

input:hover {
    border: 1px solid #814700;
}

button {
    background: #814700;
    color: white;
    font-size: 20px;
    padding: 10px;
    border: none;
    cursor: pointer;
    outline: none;
    border-radius: 20px;
}
#programme h2, #intervenants h2{
    text-align: center;
}
table {
    width: 95%;
    border-collapse: collapse;
    left: 15px;
    position: relative;
}
.intervenants{
    display: flex;
    gap: 230px;
    left: 15px;
    position: relative;
}

th, td {
    border: 1px solid #ddd;
    padding: 8px;
    text-align: center;
}
.input label{
    left: 2px;
    position: relative;
    display: block;
}
.input input{
    display: block;
    top: -20px;
    position: relative;
}
.images-nom img{
    height: 100px;
    width: 100px;
    border-radius: 50%;
    margin-bottom: 20px;
    left: 10px;
    position: relative;
}
.images-nom{
    display: grid;
}
.nom{
    left: 300px;
    top: -350px;
    position: relative;
}
.nom p{
    margin-bottom: 120px;
}