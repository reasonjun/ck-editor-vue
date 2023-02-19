<template>
  <ckeditor :editor="editor" v-model="editorData" :config="editorConfig"></ckeditor>
</template>

<script setup>
import { ref } from 'vue';
import ClassicEditor from '@ckeditor/ckeditor5-build-classic';
import '@ckeditor/ckeditor5-build-classic/build/translations/ko';

const editor = ref(ClassicEditor);
const editorData = ref('<p>Content of the editor.</p>');
const editorConfig = ref({
  // Run the editor with the Korean UI.
  language: 'ko',
});
</script>

<style scoped>

</style>
