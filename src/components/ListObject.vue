<template>
    <div class="background">
    <div class="container-wrapper">
        <h2 class="ease-title">Indeling</h2>
            <div class="list">
                <h3>Begane grond</h3>
                    <h4>Woonkamer</h4>
                        <ul>
                            <li>Compleet gemeubileerde zithoek</li>
                            <li>Eethoek</li>
                            <li>Televisie en radio</li>
                            <li>Openslaande tuindeuren naar groot terras</li>
                            <li>WiFi aanwezig</li>
                        </ul>

                    <h4>Slaapkamer</h4>
                        <ul>
                            <li>Tweepersoons boxspring</li>
                            <li>Televisie</li>
                            <li>Kastruimte</li>
                        </ul>

                    <h4>Keuken</h4>
                        <ul>
                            <li>Vaatwasser</li>
                            <li>Keramische kookplaat</li>
                            <li>Koelkast en losse diepvries</li>
                            <li>Combi oven/magnetron</li>
                            <li>Broodrooster</li>
                            <li>Complete huishoudelijke inventaris (zoals borden, glazen, bestek, etc.)</li>
                        </ul>
                    
                    <h4>Badkamer</h4>
                        <ul>
                            <li>Douche</li>
                            <li>Wastafel</li>
                            <li>Toilet</li>
                            <li>Wasmachine</li>
                        </ul>

                    <h4>Terras</h4>
                        <ul>
                            <li>Buitenterras met tuinmeubelen</li>
                        </ul>

                    <h3>Eerste verdieping</h3>

                    <h4>Slaapkamer</h4>
                        <ul>
                            <li>Twee eenpersoonsbedden</li>
                            <li>Kledingrek</li>
                        </ul>

                    <p>Bad-, bed- en keukenlinnen is aanwezig</p>

            </div>
    </div>
</div>
</template>

<style scoped>
    .background {
        width: 100%;
        background: #E5EBEA;
    }
    
    h2 {
        grid-column: 1/-1;
        grid-row: 1;
        justify-self: center;
        margin-block: var(--space-md);
    }
    .list {
        grid-column: 2/12;
        grid-row: 2;
        column-count: 1;
        margin-block-end: var(--space-md);
    }

    h4 {
        margin-inline-start: var(--space-sm);
    }

    ul {
        margin-block: var(--space-md);
    }

    li {
        font-family: var(--regular);
        font-size: var(--step--1);
        color: var(--color-text);
        }

    @media screen and (min-width: 800px) {
        .list {
            column-count: 2;
        }
    }
</style>