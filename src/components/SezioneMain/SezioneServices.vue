<script>
export default {
    name: "SezioneServices",
    data() {
        return {
            carte: [
                {
                    icona: 'fa-solid fa-sitemap',
                    servizio: 'Audit & Assurance',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {
                    icona: 'fa-solid fa-briefcase',
                    servizio: 'Financial Advisory',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {
                    icona: 'fa-solid fa-chart-simple',
                    servizio: 'Analytics and M&A',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {
                    icona: 'fa-solid fa-jet-fighter-up"></i>',
                    servizio: 'Middle Markeeting',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {
                    icona: 'fa-solid fa-globe',
                    servizio: 'Legal Consulting',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },
                {
                    icona: 'fa-solid fa-inbox',
                    servizio: 'Regulatory Risk',
                    descrizione: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.'
                },

            ]
        }
    }
}

</script>

<template>
    <div class="cont">
        <div class="box-cards">
            <div class="descrizione">
                <span>our business areas</span>
                <h2>Excellence in <span>Services</span> </h2>
                <div class="bottone d-flex align-items-center;">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Molestias officia ipsam fugit,
                        recusandae
                        natus
                        est rerum iusto quam eveniet rem provident excepturi pariatur repellendus neque odio. Unde cum ad
                        obcaecati!</p>
                    <button> see all</button>
                </div>
                <div class="cards">
                    <div class="card-body" v-for="(elem, index) in carte" :key="index">
                        <div class="internal-icons">
                            <i :class="elem.icona"></i>
                            <i class="fa-solid fa-arrow-right"></i>
                        </div>
                        <h5 class="card-title">{{ elem.servizio }}</h5>
                        <p class="card-text">{{ elem.descrizione }}</p>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.cont {
    background-color: #EEF4ED;
    padding: 40px 0 70px 0;

    .box-cards {
        width: 70%;
        margin: 0 auto;

        .cards {
            display: flex;
            flex-wrap: wrap;
            background-color: aqua;

            .card-body {
                width: calc(100% / 3);
                background-color: white;
                padding: 30px;
                border: 20px solid #EEF4ED
            }
        }
    }
}

h2 {
    span {
        color: #058283;
        background-color: #CCE3DE;
        padding: 0 10px;
    }
}

h5,
p {
    padding-top: 18px;
}

.bottone {
    p {
        padding-right: 50px;

    }

    button {
        width: 110px;
        height: 30px;
        padding: 0;
        background-color: #058283;
        color: white;
    }
}

.internal-icons {
    display: flex;
    justify-content: space-between;
    color: #058283;
    font-size: 25px;
}
</style>