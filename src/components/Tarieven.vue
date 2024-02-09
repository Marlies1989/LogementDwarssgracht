<template>
    <div class="container-wrapper" id="tarieven" >
        <h2>Tarieven</h2>
            <table class="hoogseizoen">
                <tbody>
                    <tr>
                        <th>Hoogseizoen: juli en augustus</th>
                        <th>1-2 personen</th>
                        <th>3-4 personen</th>
                    </tr>
                    <tr>
                        <td><h5>Weekendarrangement</h5>Aankomst vrijdag - vertrek maandag</td>
                        <td>€ 290</td>
                        <td>€ 395</td>
                    </tr>
                    <tr>
                        <td><h5>Midweekarrangement</h5>Aankomst maandag - vertrek vrijdag</td>
                        <td>€ 370</td>
                        <td>€ 510</td>
                    </tr>
                    <tr>
                        <td><h5>Weekarrangement</h5>Aankomst vrijdag - vertrek vrijdag</td>
                        <td>€ 610</td>
                        <td>€ 855</td>
                    </tr>
                </tbody>
            </table>

            <div class="divider"></div>

            <table class="laagseizoen">
                <tbody>
                    <tr>
                        <th>Laagseizoen: september t/m juni</th>
                        <th>1-2 personen</th>
                        <th>3-4 personen</th>
                    </tr>
                    <tr>
                        <td><h5>Weekendarrangement</h5>Aankomst vrijdag - vertrek maandag</td>
                        <td>€ 260</td>
                        <td>€ 350</td>
                    </tr>
                    <tr>
                        <td><h5>Midweekarrangement</h5>Aankomst maandag - vertrek vrijdag</td>
                        <td>€ 330</td>
                        <td>€ 450</td>
                    </tr>
                    <tr>
                        <td><h5>Weekarrangement</h5>Aankomst vrijdag - vertrek vrijdag</td>
                        <td>€ 540</td>
                        <td>€ 750</td>
                    </tr>
                </tbody>
            </table>

           <div class="info-block">
                <p>De prijzen zijn exclusief de eindschoonmaak van €55,00<br>
                    Betalingen: 20% bij reservering, restbedrag 1 week van te voren op rekening of contant bij aankomst.</p>
                <p>Aankomsttijd: vanaf 15:00 uur.<br>
                    Vertrektijd: voor 11:00 uur.</p>
                <p>Afwijkende arrangementen (dagen en tijden) zijn uitsluitend mogelijk in overleg.</p>
                <p>LET OP! Huisdieren en roken in het logement zijn niet toegestaan.</p>
           </div> 

           <a class="button" href="mailto:info@logementdwarsgracht.nl">Reserveren</a>

    </div>
</template>

<style scoped>
    h2 {
        grid-column: 1/-1;
        grid-row: 1;
        justify-self: center;
    }

    h5 {
        color: var(--color-primary);
        font-weight: bold;
    }

    th {
        font-weight: bold;
        padding-block: var(--space-sm);
    }

    td {
        padding-block: var(--space-xs);
    }

    .hoogseizoen {
        grid-column: 2 / 12;
        grid-row: 2;
        text-align: left;
    }

    .laagseizoen {
        grid-column: 2 / 12;
        grid-row: 4;
        text-align: left;
    }

    .divider {
        grid-column: 2/12;
        grid-row: 3;
        border-bottom: 2px solid var(--color-primary);
        margin-block: var(--space-xl);
    }

    .info-block {
        grid-column: 2/12;
        grid-row: 5;
        padding-block: var(--space-lg);
    }

    .info-block p {
        font-size: var(--step--2);
    }

    .button {
        grid-column: 1/-1;
        grid-row: 6;
        justify-self: center;
        background: var(--color-primary);
        padding: var(--space-sm);
        font-family: var(--title);
        font-size: var(--step-2);
        color: var(--color-secondary);
        text-decoration: none;
        box-shadow: rgba(17, 12, 46, 0.15) 0px 48px 100px 0px;
    }

    .button:hover {
        background: var(--color-white);
        color: var(--color-primary);
        text-decoration: underline solid 1px var(--color-primary);
        box-shadow: none;
    }

    #tarieven {
        margin-block-end: var(--space-md);
    }

</style>