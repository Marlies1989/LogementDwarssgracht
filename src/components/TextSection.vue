<script setup>
    defineProps(['title', 'title2'])
</script>

<template>
    <div class="container-wrapper" id="over">
        <figure class="left">
            <img src="../assets/images/riet.jpg">
        </figure>
        <div class="text-right">
            <h2>{{ title }}</h2>
            <br>
            <p>Ontdek het pittoreske Dwarsgracht, gelegen te midden van een van de meest betoverende en ongerepte natuurgebieden van Nederland: de "Weeribben-Wieden”.</p>
            <p>Ontspan volledig te midden van deze schitterende natuur, waar u de mogelijkheid hebt om heerlijk te fietsen, varen, wandelen, vissen of als u gelukt hebt in de wintermaanden te schaatsen.</p>
            <p>Elke dag wordt u verwelkomd door het gezang van vogels, het gekwaak van eenden en het geluid van kikkers. Vanuit het logement heeft u een adembenemend uitzicht op de uitgestrekte rietvelden en de schilderachtige dorpsgracht, waardoor uw verblijf nog meer betoverend wordt.</p>
        </div>
    </div>

    <div class="container-wrapper">
        <figure class="right">
            <img src="../assets/images/mus.jpg">
        </figure>
        <div class="text-left">
            <h2>{{ title2 }}</h2>
            <br>
            <p>Toen het logement in 2008 gebouwd is, is in de hele woning een aardwarmtesysteem aangelegd. Dit houdt onder anderen in dat er geen gas aansluiting aanwezig is. Op de schuur zijn 40 zonnepanelen geplaatst, deze zorgen voor de totale energie voor het logement.</p>
            <p>Overnachten in een energie neutraal logement, het kan bij ons.</p>
        </div>
    </div>
</template>

<style scoped>
figure {
    grid-column: 1 / -1;
    grid-row: 1;
    overflow: hidden;
}

img {
    width: 100%;
    object-fit: cover;
    aspect-ratio: 3/2;
}
.text-right,
.text-left {
    grid-column: 2/12;
    grid-row: 2;
    background: var(--color-white);
    text-align: center;
    padding: var(--space-xl);
    height: fit-content;
    align-self: center;
    margin-block-start: -5rem;
}

@media screen and (min-width: 800px) {
    .text-right {
    grid-column: 5/-1;
    grid-row: 1;
    margin-block-start: 0;
    }

    .text-left {
    grid-column: 1 / 9;
    grid-row: 1;
    margin-block-start: 0;
    }

    .left {
    grid-column: 1 / span 4;
    grid-row: 1;
    overflow: hidden;
    }

    .right {
    grid-column: 9 / -1;
    grid-row: 1;
    overflow: hidden;
    }

    img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    aspect-ratio: 2/3;
    }
}
</style>