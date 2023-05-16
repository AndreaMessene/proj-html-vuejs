<script>

import SezioneServices from './SezioneMain/SezioneServices.vue'
import SezioneCompany from './SezioneMain/SezioneCompany.vue'
import SezioneProjects from './SezioneMain/SezioneProjects.vue';
import SezioneRegistrazione from './SezioneMain/SezioneRegistrazione.vue';

export default {
    name: "CMainComp",
    components: {
        SezioneServices,
        SezioneCompany,
        SezioneProjects,
        SezioneRegistrazione,
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
    <section>
        <SezioneRegistrazione />
    </section>
</template>

<style lang="scss" scoped></style>