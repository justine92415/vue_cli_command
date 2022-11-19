<template>
    <div class="home">
        <img alt="Vue logo" src="../assets/logo.png" />
        <HelloWorld title="嘿嘿1" msg="fjs;fjdds"></HelloWorld>
        <HelloWorld title="嘿嘿2" msg="2"></HelloWorld>
        <HelloWorld title="嘿嘿3" msg="3"></HelloWorld>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
    name: "HomeView",
    components: {
        HelloWorld,
    },
};
</script>
