<template>
    <div class="hello" :class="type">
        <div class="img" v-for="item in 6" :key="item">
            <!-- 只接用相對路徑會出問題 -->
            <!-- <img src="../assets/logo.png" alt="" /> -->
            <img
                :src="
                    require(`@/assets/images/avatar/report_avatar_${item}.png`)
                "
                alt=""
            />
            <!-- <img src="https://picsum.photos/300/200/?random=10" /> -->
        </div>
        <div>
            <p>{{ title }}</p>
            <p>{{ msg }}</p>
            <button>搶票喔</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "HelloWorld",
    props: {
        title: String,
        msg: String,
        type: String,
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hello {
    width: 100%;
    display: inline-flex;
    margin: 1rem;
}
.img {
    width: 8rem;
    height: 8rem;
    background-color: #ddd;
}
</style>
