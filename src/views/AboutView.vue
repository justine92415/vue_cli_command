<template>
    <div class="about">
        <h1>This is an about page</h1>
        <Button type="primary">Primary</Button>
        <div>
            <Carousel v-model="value" loop>
                <CarouselItem v-for="item in 5" :key="uten">
                    <div class="demo-carousel">
                        <img
                            :src="
                                require(`@/assets/images/avatar/report_avatar_${item}.png`)
                            "
                            alt=""
                        />
                    </div>
                </CarouselItem>
            </Carousel>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            value: 0,
        };
    },
};
</script>
