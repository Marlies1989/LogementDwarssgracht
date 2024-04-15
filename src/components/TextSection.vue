<script setup>
    defineProps(['title', 'title2', 'title3'])
</script>

<template>
    <div class="container-wrapper text" id="over">
        <figure class="left">
            <img src="../assets/images/riet.jpg">
        </figure>
        <div class="text-right">
            <h2>{{ title }}</h2>
            <br>
            <p>Logement ‘Dwarszicht’ is gelegen in het pittoreske dorpje Dwarsgracht ±3km ten westen van Giethoorn. Midden in de Weeribben-Wieden gesitueerd in het achterhuis van een in 2008 nieuw gebouwde woonboerderij van de familie Petter, komt u heerlijk tot rust.</p> 
            <p>Het logement ligt vanaf de openbare weg gezien aan de overkant van de dorpsgracht, maar desondanks zeer goed bereikbaar via een karakteristieke brug over het water.</p>
            <p>Elke dag wordt u verwelkomd door het gezang van vogels, het gekwaak van eenden en het geluid van kikkers. Vanuit het logement en vanaf het terras heeft u uitzicht over de tuin, de rietvelden en het water. Een idyllisch decor dat zich leent voor het bewonderen van prachtige zonsondergangen.</p>
        </div>
    </div>

    <div class="container-wrapper text">
        <figure class="right">
            <img src="../assets/images/mus.jpg">
        </figure>
        <div class="text-left">
            <h2>{{ title2 }}</h2>
            <br>
            <p>
Het logement bevindt zich in een gerenoveerde woonboerderij, die in 2008 volledig herbouwd is. De hele woonboerderij wordt aangedreven door een gesloten aardwarmtesysteem, wat betekent dat er geen gasaansluiting aanwezig is. Bovendien zijn er 40 zonnepanelen op de schuur geïnstalleerd, die voorzien in de totale energiebehoefte van zowel het logement als de woonboerderij.</p>
            <p>Overnachten in een energie neutraal logement, het kan bij ons.</p>
        </div>
    </div>

    <div class="container-wrapper text">
        <figure class="left">
            <img src="../assets/images/sloep_varen.jpg">
        </figure>
        <div class="text-right">
            <h2>{{ title3 }}</h2>
            <br>
            <p>Wilt u de prachtige omgeving via het water verkennen? Maak dan een tochtje met de kano die bij het logement hoort.</p>
            <p>Of huur/reserveer ter plekke een luxe elektrisch aangedreven sloep via <a href="https://www.pettersloepverhuur.nl/" target="_blank">Petter sloepverhuur.</a></p>
        </div>
    </div>
</template>

<!-- <script>
  import gsap from "gsap";
  import { ScrollTrigger } from "gsap/ScrollTrigger";
  gsap.registerPlugin(ScrollTrigger);

  export default {
  mounted() {    
      ScrollTrigger.batch('.text', {
        onEnter: batch => {
            gsap.from(batch, { y: 100, stagger: .25})
            },
        });
  }
};
</script> -->

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
    padding: var(--space-md);
    height: fit-content;
    align-self: center;
    margin-block-start: -5rem;
}

@media screen and (min-width: 800px) {
    .text-right {
    grid-column: 5/-1;
    grid-row: 1;
    margin-block-start: 0;
    padding: var(--space-xl);
    }

    .text-left {
    grid-column: 1 / 9;
    grid-row: 1;
    margin-block-start: 0;
    padding: var(--space-xl);
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