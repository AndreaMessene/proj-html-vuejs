<script>

import SezioneServices from './SezioneMain/SezioneServices.vue'
import SezioneCompany from './SezioneMain/SezioneCompany.vue'

export default {
    name: "CMainComp",
    components: {
        SezioneServices,
        SezioneCompany
    },
}

</script>

<template>
    <section>
        <SezioneServices />
    </section>
    <section>s
        <SezioneCompany />
    </section>
</template>

<style lang="scss" scoped></style>