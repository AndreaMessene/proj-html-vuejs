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
    <div class="box d-flex">
        <div class="company">
            <div class="box-company">
                <span class="short-text">
                    about the network
                </span>

                <h2> <span>The</span> Company</h2>

                <p>For 12Years we have been providing audit and warranty, financial advice, risck advice, texas
                    and related
                    service to select clients</p>
                <div class="box-info">
                    <div class="for-info" v-for="(elem, index) in companyIcons" :key="index">
                        <h4><i :class="elem.icona"></i>{{ elem.nome }}</h4>
                        <p>{{ elem.text }}</p>
                    </div>
                </div>
                <div class="for-button ">
                    <div class="d-flex">
                        <a href="" v-for="(elem, index) in button" :key="index"> {{ elem.nome }} </a>
                    </div>


                </div>
            </div>
        </div>

        <div class="img-cont company">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.box {
    .company {
        width: calc(100% / 2);
        background-color: #111117;
        color: white;
        display: flex;
        justify-content: flex-end;

        .box-company {
            width: 68%;
            padding: 20px;


            .short-text {
                color: #058283;
                display: block;
                font-size: 12px;
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

            .box-info {
                display: flex;
                flex-wrap: wrap;


                .for-info {
                    width: calc(100% / 2);

                    h4 {
                        font-size: 17px;

                        i {
                            padding-right: 13px;
                            color: #058283;
                        }
                    }

                }
            }

            .for-button {
                div {
                    margin-left: -40px;

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
        }

        p {
            font-size: 12px;
            padding: 15px 0;
        }
    }

    .img-cont {

        background-image: url('/img/sfondo/about-4.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }
}
</style>