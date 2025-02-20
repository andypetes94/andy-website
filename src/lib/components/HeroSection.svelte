<script>
    import Logo from "$assets/DS_Logo1.png";
    import { Button } from "$components";
    //import shite from "./../../assets/DS_logo.png";
</script>


<section class="hero">
    <div class="hero-showcase text-center bold">
        <h1 class="logo-purple mb-s">Vizify</h1>
        <img class = "logo mb-s" src={Logo} alt="" />
        <h3 class = "logo-purple">Simplifying Data, Amplifying Impact</h3>
    </div>


    <div class="hero-text white text-center">
        <h2 class="mb-l">Unlock the Power of Your Data with Stunning Visualisations</h2>
        <p class="mb-l">Transform your raw data into compelling, insightful visuals that drive decisions and tell a powerful story. Whether you need interactive dashboards, engaging reports, or custom data visualisations, we specialise in turning complex datasets into clear, actionable insights.</p>
        <Button>Purchase Now!</Button>
    </div>


</section>

<style>
    .hero {
        display: flex;
        height: 100vh;
        overflow-y: "hidden";
    }

    .hero-showcase {
        position: relative;
        width: 50%;
        padding: 100px 16px 0 16px;
        background: linear-gradient(
            135deg,
            #99fdf2,
            #ccfcf6 25%,
            #d8f5fa 50%,
            #9ffbf1 75%,
            #88fbee

        );
    }

    .hero-text {
        width: 50%;
        padding: 100px 5%;
        background: black;
    }

    .logo {
        
        width: 50%;

        right: 25%;
        left: 25%;

    }


</style>