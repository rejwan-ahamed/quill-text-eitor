<template>
    <h1>text</h1>
    <QuillEditor toolbar="full" />
    <input type="text" v-model="test" >
    <button v-on:click="show()">submit</button>
</template>

<script>
import { QuillEditor } from '@vueup/vue-quill'
import '@vueup/vue-quill/dist/vue-quill.snow.css';
export default {
    name: 'MainText',
    components: {
        QuillEditor
    },
    data() {
        return {
        test:'',
        }
    },
    methods:{
        show(){
            const datamain = this.test
            alert(datamain)
        }
    }
}
</script>

<style>
</style>