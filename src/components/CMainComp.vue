<script>
export default {
    name: "BaNavComp",
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
    <div class="container">
        <div class="descrizione">
            <span>our business areas</span>
            <h2>Excellence in Service</h2>
            <div class="bottone">
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Molestias officia ipsam fugit, recusandae natus
                    est rerum iusto quam eveniet rem provident excepturi pariatur repellendus neque odio. Unde cum ad
                    obcaecati!</p>
                <button> see all</button>
            </div>
            <div class="cards">
                <div class="card">
                    <div class="card-body" v-for="(elem, index) in carte" :key="index">
                        <div>
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
div {
    background-color: green;
}
</style>