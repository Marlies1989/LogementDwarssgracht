<template>
    <div class="container-wrapper" id="fotos">
        <div class="photo-2">
            <figure>
                <img src="../assets/images/terras_dg.jpeg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/logement.jpeg" alt="">
            </figure>
        </div>
        <div class="photo-4">
            <figure>
                <img src="../assets/images/mus.jpg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/Winter_logement_dg.jpeg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/riet.jpg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/schaatsen_dg.jpeg" alt="">
            </figure>
        </div>
        <div class="photo-4">
            <figure>
                <img src="../assets/images/eenden_dg.jpeg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/zwanen_dg.jpeg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/otter_dg.jpg" alt="">
            </figure>
            <figure>
                <img src="../assets/images/ooienvaar_dg.jpeg" alt="">
            </figure>
        </div>
    </div>
</template>

<style scoped>
 .photo-2 {
    grid-column: 1/-1;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    gap: var(--space-md);
    margin-block-end: var(--space-md);
 }

 .photo-4 {
    grid-column: 1/-1;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    gap: var(--space-md);
    margin-block-end: var(--space-md);
 }

 img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    aspect-ratio: 1/1;
 }

 @media screen and (min-width: 608px) {
    .photo-2 {
        grid-template-columns: repeat(auto-fill, minmax(calc(500px - var(--space-md)), 1fr));
    }

    .photo-4 {
        grid-template-columns: repeat(auto-fill, minmax(calc(320px - var(--space-md)), 1fr));
    }

 }

</style>