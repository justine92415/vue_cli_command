<template>
    <div class="about">
        <Images link="https://fakeimg.pl/100"></Images>
        <Images link="https://fakeimg.pl/150"></Images>
        <h1>This is an news page</h1>
        <HelloWorld title="緊張喔" type="wide"></HelloWorld>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Images from "@/components/Images.vue";

export default {
    name: "NewsView",
    components: {
        HelloWorld,
        Images,
    },
};
</script>
