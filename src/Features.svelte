<script>
    let img1 = "/img/features_1.png";
    let icon1 = "/img/icon_1.svg";
    let icon2 = "/img/icon_2.svg";
    let icon3 = "/img/icon_3.svg";
    let icon4 = "/img/icon_4.svg";
</script>

<section id="features">
    <h1>The new amazing features</h1>

    <div class="row">
        <div class="left">
            <img src={img1} alt="Img_features" />
        </div>

        <div class="right">
            <div class="right-item">
                <img src={icon1} alt="Icon" />
                <span>
                    <h4>60 fps</h4>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    </p>
                </span>
            </div>

            <div class="right-item">
                <img src={icon2} alt="Icon" />
                <span>
                    <h4>30 fps</h4>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    </p>
                </span>
            </div>

            <div class="right-item">
                <img src={icon3} alt="Icon" />
                <span>
                    <h4>1 inch image sensor</h4>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    </p>
                </span>
            </div>

            <div class="right-item">
                <img src={icon4} alt="Icon" />
                <span>
                    <h4>10 hours battery life</h4>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    </p>
                </span>
            </div>
        </div>
    </div>
</section>
