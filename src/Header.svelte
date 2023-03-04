<script>
    
    function scrollToBottom() {
        window.scrollTo(0, document.body.scrollHeight);
    }

    function myFunction() {
        // let i = document.getElementsByTagName("i");
        let x = document.getElementById("myTopnav");
        if (x.className === "topnav") {
            x.className += " responsive";
        } else {
            x.className = "topnav";
        }
    }

    let logo = "/img/logo.png";
    let img_drone = "/img/drone.png";
</script>

<header id="header">
    <div class="container">
        <div class="topnav" id="myTopnav">
            <a href="#"><img src={logo} alt="Logo" /></a>

            <a class="icon" id="Icon" on:click={myFunction}>
                <i class="fa fa-bars" />
            </a>

            <nav>
                <a href="#header" class="active">Home</a>
                <a href="#about">About</a>
                <a href="#features">Features</a>
                <a href="#gallery">Gallery</a>
                <a href="#testimonials">Testimonials</a>
            </nav>
        </div>

        <div class="container-row">
            <div class="left">
                <img src={img_drone} alt="Drone" />
            </div>

            <div class="right">
                <h1>Drone?</h1>
                <h1>You Need a REFLEX 3</h1>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. A
                    dictum nunc faucibus eget eu. Morbi eu proin feugiat magna
                    nam.
                </p>
                <div class="right-button">
                    <button class="button button-1">Buy now</button>
                    <button class="button button-2">More details</button>
                </div>
            </div>
        </div>
        <div class="chevron-down" on:click={scrollToBottom}>
            <a href="#" class="icon-down">
                <i class="fa-solid fa-chevron-down" />
            </a>
        </div>
    </div>
</header>
