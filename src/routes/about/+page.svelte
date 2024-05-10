<section>
    <h1>Beauty</h1>
    <p>Beauty is when I feel my heart drop into a bottomless pit.</p>
    <p>Beauty comes in many forms.</p>
    <p>To me, beauty is the emotional resonance of a film and its music.</p>
    <p>Beauty is an attractive person in attractive clothing.</p>
    <p>
        Beauty is an interactive software experience that feels new, unique,
        and perfect.
    </p>
    <h1>About</h1>
    <p>My life's work is to understand and create beauty.</p>
    <p>This is why I play the soundtracks of my favorite films on piano.</p>
    <p>
        It's why I compose my own music and write my own screenplays, short
        stories, and essays.
    </p>
    <p>
        It's why I'm learning everything I can about fashion and the fashion
        industry.
    </p>
    <p>It's why I build software products.</p>
    <p><a href="/" style="color: black">Home</a></p>
</section>

<style>
    @font-face {
        font-family: "EB Garamond";
        src: url("EBGaramond-VariableFont_wght.ttf") format("truetype");
        font-weight: normal;
        font-style: normal;
    }
    :global(body) {
        font-family: "EB Garamond", serif;
        background-color: rgb(236, 236, 236);
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0;
        padding: 0;
    }
    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: left;
        padding: 0 48px;
        display: flex;
        background-color: white;
        margin: 16px;
        padding-bottom: 36px;
        box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
    }
    section {
        opacity: 0;
        transform: translateY(-32px);
        animation: slide-down 0.7s ease-out forwards;
    }
    @keyframes slide-down {
        0% {
            opacity: 0;
            transform: translateY(-32px);
        }
        100% {
            opacity: 1;
            transform: translateY(0);
        }
    }
    h1 {
        font-family: "EB Garamond";
        font-size: 2.6em;
    }
    p {
        font-family: "EB Garamond";
        font-size: 1.3em;
    }
</style>
