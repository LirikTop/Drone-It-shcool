<script>
    let img = "/img/order.png";
</script>

<section id="order">
    <div class="row">
        <div class="left">
            <img
                src={img}
                alt="copter"
                data-aos="fade-right"
                data-aos-duration="5000"
                data-aos-offset="300"
                data-aos-easing="ease-in-sine"
            />
        </div>
        <div
            class="right"
            data-aos="fade-left"
            data-aos-offset="300"
            data-aos-duration="3000"
            data-aos-easing="ease-in-sine"
        >
            <h2>Order now</h2>
            <div>
                <input
                    placeholder="Name"
                    class="input"
                    name="text"
                    type="text"
                />
                <input
                    placeholder="Telephon"
                    class="input"
                    name="text"
                    type="tel"
                />
            </div>
            <button class="custom-btn btn-1">Submit</button>
        </div>
    </div>
</section>
