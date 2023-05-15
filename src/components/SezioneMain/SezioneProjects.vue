<script>
export default {
    name: "SezioneProjects",
    data() {
        return {
            cards: [
                {
                    img: "/img/luoghi/project-1.jpg",
                    info: "Academic professional program in social media"
                },
                {
                    img: "/img/luoghi/project-2.jpg",
                    info: "Presidnt's speech at the annual meeting"
                },
                {
                    img: "/img/luoghi/project-3.jpg",
                    info: "International business trip in shanghai"
                },
                {
                    img: "/img/luoghi/project-4.jpg",
                    info: "Technology workshop whit education theme"
                },
                {
                    img: "/img/luoghi/project-5.jpg",
                    info: "Donation of clothes and food to the partner NGO"
                },
                {
                    img: "/img/luoghi/project-6.jpg",
                    info: "Confraternization of the procurement team"
                },
            ],

            link: [
                { nome: "all" },
                { nome: "institutiola" },
                { nome: "social" },
                { nome: "events" },
                { nome: "innovation" },
                { nome: "environment" },
                { nome: "technology" },
            ]
        }
    }

}

</script>

<template>
    <div class="cont">
        <header>
            <p>we do more for everyone</p>
            <h3>Action & <span>Prejects</span></h3>
        </header>
        <nav>
            <div>
                <ul>
                    <li v-for="(elem, index) in link" :key="index">
                        <a href="#">{{ elem.nome }}</a>
                    </li>
                </ul>
            </div>
        </nav>
        <main>
            <div class="cards" v-for="(elem, index) in cards" :key="index">
                <img :src="elem.img" alt="pc">
                <p>{{ `${elem.info}` }}</p>
            </div>
        </main>
    </div>
</template>

<style lang="scss" scoped>
.cont {
    width: 70%;
    margin: 0 auto;
    padding: 6rem 0;
    display: flex;
    flex-direction: column;
    align-items: center;

    header {
        p {
            color: #00A6AC;
            text-align: center;
        }

        h3 {
            padding: 10px 0 35px 0;

            span {
                color: #058283;
                background-color: #DAECED;

            }
        }
    }

    nav {
        width: 70%;
        padding-bottom: 10px;

        div {
            ul {
                display: flex;
                justify-content: space-between;

                li {
                    list-style: none;


                    a {
                        text-decoration: none;
                        color: gray;
                        padding: 5px;

                        &:hover {
                            background-color: #DAECED;
                            border-radius: 5px;
                            padding: 5px;
                        }
                    }
                }
            }
        }
    }

    main {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;

        .cards {
            width: calc(100% / 3 - 20px);
            height: 250px;
            margin-bottom: 20px;
            position: relative;


            img {
                width: 100%;
                height: 100%;
                border-radius: 10px;
                filter: brightness(60%);
            }

            p {
                width: 80%;
                position: absolute;
                bottom: 0px;
                left: 25px;
                color: white;
                font-weight: bold;
            }
        }
    }
}
</style>

