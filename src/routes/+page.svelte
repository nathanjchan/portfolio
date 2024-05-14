<script>
    function handleNameClick() {
        window.location.href = "/about";
    }
    function handleRemyntClick() {
        window.location.href = "https://www.loom.com/share/272a6fc803574061a0fe42a73b24b93b?sid=d70f09fa-94ae-4c94-b306-1a412f0b1e73";
    }
    function handleDominoClick() {
        window.location.href = "/domino";
    }
    function handleNextnavClick() {
        window.location.href = "https://nextnav.com";
    }
    function handleCmbClick() {
        window.location.href = "https://mindbrain.ucdavis.edu/";
    }
</script>

<svelte:head>
    <title>Nathan Chan Portfolio</title>
    <meta name="description" content="Nathan Chan Portfolio" />
</svelte:head>

<container>
    <vdiv>
        <section style="animation-delay: 0s;">
            <h1 on:click={handleNameClick} on:keydown={() => {}}>
                Nathan Chan
            </h1>
            <p>Portfolio</p>
        </section>
        <section style="animation-delay: 0.1s;">
            <img
                class="remynt-cropped"
                src="remynt-logo.png"
                alt="Remynt logo"
                on:click={handleRemyntClick}
                on:keydown={() => {}}
            />
            <p>Founding Engineer</p>
        </section>
    </vdiv>
    <section2x2 style="animation-delay: 0.2s;">
        <vdiv>
            <img
                class="domino-cropped"
                src="domino-sign-in.png"
                alt="Domino sign in"
                on:click={handleDominoClick}
                on:keydown={() => {}}
            />
            <p>
                Built a video-based social media iOS app with video-sharing
                features and video editing tools.
            </p>
        </vdiv>
    </section2x2>
    <section2x2 style="animation-delay: 0.3s;">
        <vdiv>
            <!-- <domino-cropped
                on:click={handleDominoClick}
                on:keydown={() => {}}
            /> TODO: replace with Lamar Health screenshot. -->
            <p>
                Built a health-tracking app in React Native.
            </p>
        </vdiv>
    </section2x2>
    <vdiv>
        <section style="animation-delay: 0.4s;">
            <nextnav-logo
                on:click={handleNextnavClick}
                on:keydown={() => {}}
            />
            <p>Software Engineer</p>
        </section>
        <section style="animation-delay: 0.5s;">
            <img
                class="cmb-logo"
                src="cmb-logo.png"
                alt="CMB logo"
                on:click={handleCmbClick}
                on:keydown={() => {}}
            />
            <p>Research Assistant</p>
        </section>
    </vdiv>
</container>

<style>
    :global(body) {
        background-color: rgb(236, 236, 236);
    }
    container {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
    }
    vdiv {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    section,
    section2x2 {
        opacity: 0;
        transform: translateY(32px);
        animation: slide-up 0.7s ease-out forwards;
    }
    @keyframes slide-up {
        0% {
            opacity: 0;
            transform: translateY(32px);
        }
        100% {
            opacity: 1;
            transform: translateY(0);
        }
    }
    .remynt-cropped {
        width: 166px;
        height: 56px;
        background-image: url("remynt-logo.png");
        margin: auto;
        margin-bottom: 8px;
        margin-top: 0px;
        transition: transform 0.4s ease;
    }
    .remynt-cropped:hover {
        transform: scale(1.05);
        cursor: pointer;
    }
    .domino-cropped {
        width: 300px;
        height: 300px;
        object-fit: cover;
        object-position: 0 -75px;
        margin-bottom: 16px;
        transition: transform 0.4s ease;
    }
    .domino-cropped:hover {
        transform: scale(1.03);
        cursor: pointer;
    }
    .cmb-logo {
        width: 150px;
        transition: transform 0.4s ease;
    }
    .cmb-logo:hover {
        transform: scale(1.05);
        cursor: pointer;
    }
    nextnav-logo {
        width: 240px;
        height: 80px;
        background-image: url("nextnav-logo.jpeg");
        background-position: 0 -22px;
        background-size: cover;
        transition: transform 0.4s ease;
        margin-bottom: 8px;
    }
    nextnav-logo:hover {
        transform: scale(1.05);
        cursor: pointer;
    }
    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 312px;
        height: 208px;
        text-align: center;
        background-color: white;
        border-radius: 30px;
        margin: 8px;
    }
    section2x2 {
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 640px;
        height: 432px;
        text-align: center;
        background-color: white;
        border-radius: 30px;
        margin: 8px;
    }
    h1 {
        margin: 0;
        font-size: 2.6em;
        font-family: Helvetica;
        background: linear-gradient(90deg, rgb(129 129 129), rgb(44 44 44));
        -webkit-background-clip: text;
        background-clip: text;
        -webkit-text-fill-color: transparent;
        padding: 0 16px;
        transition: transform 0.4s ease;
    }
    h1:hover {
        transform: scale(1.05);
        cursor: pointer;
    }
    p {
        margin: 0;
        font-size: 1.3em;
        font-family: Helvetica;
        padding: 0 16px;
    }
</style>
