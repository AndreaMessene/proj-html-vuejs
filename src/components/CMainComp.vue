<script>

import SezioneServices from './SezioneMain/SezioneServices.vue'
import SezioneCompany from './SezioneMain/SezioneCompany.vue'
import SezioneProjects from './SezioneMain/SezioneProjects.vue';

export default {
    name: "CMainComp",
    components: {
        SezioneServices,
        SezioneCompany,
        SezioneProjects
    },
}

</script>

<template>
    <section>
        <SezioneServices />
    </section>
    <section>
        <SezioneCompany />
    </section>
    <section>
        <SezioneProjects />
    </section>
</template>

<style lang="scss" scoped></style>