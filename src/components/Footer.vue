<script>
    export default {
  name: 'FooterSection',
};
</script>

<template>
<div class="background" id="contact">
    <div class="container-wrapper">
        <h2>Contact</h2>
            <address>
                Logement Dwarsgracht <br>
                Dwarsgracht 21 <br>
                8355 CT Giethoorn
            </address>
            <div class="contact-info">
                <a href="tel:+31627166054">+31 6 27 16 60 54</a><br>
                <a href="mailto:info@logementdwarsgracht.nl">info@logementdwarsgracht.nl</a><br>
                <a href="https://www.google.nl/maps/dir//Vakantiehuisje+Dwarsgracht,+Logement+Dwarszicht,+Dwarsgracht+21,+8355+CT+Giethoorn/@52.7237647,5.9537151,12z/data=!4m9!4m8!1m0!1m5!1m1!1s0x47c86fe3b3c2783d:0x6130fed6da3c11cb!2m2!1d6.0362878!2d52.7236894!3e0?entry=ttu>">Google Maps route</a>
            </div>
    </div>
</div>
   
</template>

<style scoped>
    .background {
        width: 100%;
        background: var(--color-blue);
        height: 100%;
    }
    .container-wrapper {
        padding: var(--space-md);
        margin-block-end: 0;
    }

    h2 {
        color: var(--color-secondary);
        grid-column: 2;
    }

    address {
        grid-column: 2 / -1;
        grid-row: 2;
        color: var(--color-secondary);
        font-family: var(--regular);
        font-style: normal;
    }

    .contact-info {
        grid-column: 2 / -1;
        grid-row: 3;
    }

    .contact-info a {
        color: var(--color-secondary);
        font-family: var(--regular);
        font-style: normal;
    }

    @media screen and (min-width: 800px) {
        address {
            grid-column: 2/5;
        }

        .contact-info {
            grid-column: 6 / -1;
            grid-row: 2;
        }
    }
</style>