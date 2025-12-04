<script lang="ts">
 import { onMount } from "svelte";

 onMount(()=>{
    const defaultTheme = window.matchMedia("(prefers-color-scheme: dark)").matches? 'dark':'ligth';
    document.documentElement.setAttribute('data-theme',defaultTheme);
 });
</script>