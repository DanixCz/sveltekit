<section class="hero">
    <div>
        <img src=https://www.farnostkralupy.cz/nockostelu/wp-content/uploads/sites/2/2021/03/Kralupy-kostel-oltar-1024x601.jpg alt="">
    </div>

    <img src=https://cdn.myshoptet.com/usr/www.zuty.cz/user/shop/big/16550-3_malovani-podle-cisel-jezis-kristus.png?65006088 alt="">

    <h1>Ježíš Kristus</h1>

    <p>Pojďte stavět vaší budoucnost</p>

    <div class="hero-buttons">

        <a href="/about">Login</a>

        <a href="/" id="ghost">About</a>
        <!--
            Druhý odkaz se stejným HTML tagem <a>, tentokrát s id "ghost", což ho odlišuje pro stylování.
            ID je jedinečný identifikátor elementu na stránce.
        -->
    </div>
</section>

<style>
    .hero {
        width: 100%; /* Nastavuje šířku sekce na 100 % šířky okna. */
        min-height: calc(100vh - 100px); /* Výška sekce je minimálně rovna výšce okna mínus 100px. */
        max-width: 1300px; /* Maximální šířka sekce je omezena na 1300px. */
        display: flex; /* Použití Flexboxu pro uspořádání elementů. */
        flex-direction: column; /* Uspořádání elementů ve sloupci (svisle). */
        justify-content: center; /* Vertikální vycentrování obsahu. */
        align-items: center; /* Horizontální vycentrování obsahu. */
        text-align: center; /* Text uvnitř sekce je zarovnán na střed. */
    }

    .hero img {
        width: 250px; /* Nastavení pevné šířky obrázku na 250 pixelů. */
        border-radius: 20px;
    }

    .hero-buttons {
        display: flex; /* Použití Flexboxu pro uspořádání tlačítek. */
        gap: 36px; /* Mezera 36px mezi tlačítky. */
    }
    .hero p {
        padding-bottom: 30px;
    }

    .hero-buttons a {
        color: white; /* Barva textu je bílá. */
        background-color: rgb(221, 37, 37); /* Zelená barva pozadí tlačítka. */
        text-decoration: none; /* Odstranění podtržení odkazu. */
        width: 150px; /* Pevná šířka tlačítka je 150px. */
        height: 50px; /* Pevná výška tlačítka je 50px. */
        display: flex; /* Flexbox pro snadné zarovnání obsahu uvnitř tlačítka. */
        justify-content: center; /* Horizontální vycentrování textu uvnitř tlačítka. */
        align-items: center; /* Vertikální vycentrování textu uvnitř tlačítka. */
        border-radius: 10px; /* Zaoblení rohů tlačítka na 10px. */
        font-weight: 500; /* Středně tučné písmo. */
        font-family: Arial, Helvetica, sans-serif; /* Font pro tlačítka. */
        transition: ease 0.5s; /* Přechod pro animaci při změně stylu (0.5 sekundy). */
    }

    #ghost {
        color: black; /* Černá barva textu. */
        background: none; /* Žádné pozadí tlačítka. */
        border: 1px solid black; /* Černý rámeček kolem tlačítka. */
        transition: ease 0.5s; /* Přechod při změně stylu (0.5 sekundy). */
    }

    #ghost:hover {
        color: white; /* Text se změní na bílý při najetí myší. */
        background: rgb(69, 165, 243); /* Pozadí tlačítka se změní na červené při najetí myší. */
        border: 1px solid rgba(0,0,0,0); /* Rámeček tlačítka zmizí (průhledný) při najetí myší. */
    }

    .hero-buttons a:hover {
        color: white; /* Text se změní na bílý. */
        background: rgb(69, 165, 243); /* Pozadí se změní na červené. */
    }

</style>
