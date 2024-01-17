<template>
    <div class="container-wrapper">
        <figure>
            <img src="../assets/images/logement.jpeg">
        </figure>
        <div class="hero-text">
            <p>Logement ‘Dwarszicht’ is gelegen in het pittoreske dorpje Dwarsgracht ±3km ten westen van Giethoorn en gesitueerd in het achterhuis van een in 2008 nieuw gebouwde woonboerderij van de familie Petter.</p> 
            <p> Het logement ligt in de midden buurt van Dwarsgracht. Vanaf de openbare weg gezien aan de overkant van de dorpsgracht maar desondanks zeer goed bereikbaar via een karakteristieke brug over het water.</p>
        </div>
    </div>
</template>

<style scoped>
figure {
    grid-column: 1 / -1;
    grid-row: 1;
}

img {
    width: 100dvw;
}
.hero-text {
    grid-column: 2/12;
    grid-row: 2;
    z-index: 100;
    background: rgba(255, 255, 255, 0.90);
    box-shadow: 0px 2px 50px 5px rgba(0, 0, 0, 0.05);
    text-align: center;
    padding: var(--space-md);
    height: fit-content;
    align-self: center;
    margin-block-start: -5rem;
}

@media screen and (min-width: 800px) {
    .hero-text {
        grid-column: 8/-1;
        grid-row: 1;
        margin-block-start: 0;
        padding: var(--space-xl);
    }

    figure {
        grid-column: 1 / span 10;
        grid-row: 1;
        overflow: hidden;
    }

    img {
        height: 90vh;
        width: auto;
    }

}
</style>