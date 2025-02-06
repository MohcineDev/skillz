<script setup>
</script>
<template>
    <section>
        <div class="container">
            <div>

                <h2>Lorem ipsum dolor sit amet consectetur ipsum dolor sit ?</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum, illum cum. Error, amet quae possimus
                    consectetur, laudantium autem ea minima corporis fugit eligendi inventore nesciunt non animi
                    expedita quas omnis?</p>
            </div>
            <div>
                <div class="card">
                    <div>
                        <div class="title">
                            <img src="../assets/social-media.png" alt="">
                            <h3>100% satisfaction</h3>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
                    </div>
                    <div>
                        <div class="title">
                            <img src="../assets/working.png" alt="">
                            <h3>4 years of experience</h3>
                        </div>

                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
                    </div>
                    <div>
                        <div class="title">
                            <img src="../assets/work-in-progress.png" alt="">
                            <h3>expert teams members</h3>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
                    </div>
                    <div>
                        <div class="title">

                            <img src="../assets/global-connection.png" alt="">
                            <h3>expert teams members</h3>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>
<style scoped>
section{
    padding: 4rem 0;
}
.container {
    max-width: var(--max-width);
    display: flex;
    margin: auto;
    gap: 30px;
    align-items: center;
}

.container>div {
    flex: 1;
}

.card {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
}

h2 {
    font-size: 2rem;
}

.title {
    display: flex;
}

.card>div {
    margin: 2rem 0;
}

.card img {
    width: 50px;
    height: 50px;
    margin: 10px;
}

p {
    color: #888;
}
</style>