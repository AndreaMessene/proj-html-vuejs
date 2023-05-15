<script >

export default {
    name: "SezioneCompany",
    data() {
        return {
            companyIcons: [
                {
                    icona: "fa-solid fa-medal",
                    nome: "Tradition",
                    text: "lorem ipsum dolor sit amet conseccteur adipiscing alit"
                },
                {
                    icona: "fa-solid fa-lock",
                    nome: "Security",
                    text: "lorem ipsum dolor sit amet conseccteur adipiscing alit"
                },
                {
                    icona: "fa-regular fa-pen-to-square",
                    nome: "Certificate",
                    text: "lorem ipsum dolor sit amet conseccteur adipiscing alit"
                },
                {
                    icona: "fa-solid fa-graduation-cap",
                    nome: "Experties",
                    text: "lorem ipsum dolor sit amet conseccteur adipiscing alit"
                },
            ],

            button: [
                {
                    nome: "get in touch"
                },
                {
                    nome: "read more"
                }
            ]
        }
    }
}


</script>

<template>
    <div class="cont d-flex">
        <div class="company">
            <span class="short-text">
                about the network
            </span>

            <h2> <span>The</span> Company</h2>

            <p>For 12Years we have been providing audit and warranty, financial advice, risck advice, texas and related
                service to select clients</p>
            <div>
                <div class="for-info" v-for="(elem, index) in companyIcons" :key="index">
                    <h3><i :class="elem.icona"></i>{{ elem.nome }}</h3>
                    <p>{{ elem.text }}</p>
                </div>

            </div>
            <div class="for-button d-flex ">
                <a href="" v-for="(elem, index) in button" :key="index"> {{ elem.nome }} </a>

            </div>
        </div>

        <div class="img-cont company">
        </div>

    </div>
</template>

<style lang="scss" scoped>
.cont {
    width: 70%;
    height: 400px;
    margin: 0 auto;

    .company {
        width: calc(100% / 2);
        background-color: #111117;
        color: white;

        .short-text {
            color: #058283;
            display: block;
        }

        h2 {
            span {
                background-color: #03848443;
                padding: 7px 7px;

            }
        }

        span,
        h2,
        p {
            margin-bottom: 20px;
        }

        .for-info {}

        .for-button {
            a {
                color: white;
                text-decoration: none;
                padding: 5px 8px;
                border: 2px solid #058283;
                ;


                &:first-child {
                    background-color: #058283;
                    margin: 0 25px 0 40px;
                }
            }
        }
    }

    .img-cont {

        background-image: url('/img/sfondo/about-4.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }
}
</style>