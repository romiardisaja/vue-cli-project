<template>
    <h2>{{ judul }}</h2>
    <button @click="changeJudul">Ubah Judul</button>
</template>

<script>
export default {
    name: 'Header',
    props: ['judul'],
    data() {
        return {
            newJudul: "Judul baru dari Header.vue"
        }
    },
    methods: {
        changeJudul(){
            this.$emit('headerChangeJudul', this.newJudul)
        }
    },
    emits: ['headerChangeJudul']
}
</script>

<style>

</style>