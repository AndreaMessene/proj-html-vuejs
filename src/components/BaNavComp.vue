<script>
export default {
    name: "BaNavComp",
    data() {
        return {
            link: [
                {
                    nome: "home"
                },
                {
                    nome: "service"
                },
                {
                    nome: "about"
                },
                {
                    nome: "projects"
                },
                {
                    nome: "results"
                }
            ]
        }


    }
}



</script>

<template>
    <div class="container">
        <img src="/img/loghi/logo.png" alt="logo">
        <div>
            <ul>
                <li v-for="(element, index) in link" :key="index">
                    <a href="#"> {{ element.nome }} </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    width: 50%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 15px 0 15px 0;

    img {
        height: 30px;

    }

    div {
        ul {
            display: flex;
            margin-bottom: 0px;

            li {
                list-style: none;
                // padding: 15px 10px 0 10px;
                margin: 5px;


                a {
                    text-decoration: none;
                }
            }
        }
    }
}
</style>