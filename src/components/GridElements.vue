<template lang="">
    <div class="grid-elements">
        <div class="" v-for="(item, index) in content.icons" :key="index">
            <div class="grid-item">
                <h4>{{item}}</h4>
                <h5>{{content.body[index]}}</h5>
            </div>
        
        </div>

    </div>
</template>
<script>
export default {
    data() {
        return {
            content: {
                icons: [1, 2, 3, 4, 5, 6],
                body: ["Name 1", "Name 2", "Name 3", "Name 4", "Name 5", "Name 6"]

            }
        }
    },
}
</script>
<style scoped>
.grid-elements {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-gap: 2rem;
    grid-auto-columns: 1fr;
    grid-auto-rows: 1fr;
    grid-template-areas:
        "a b c"
        "d e f";
    place-items: center;
    height: 50vh
}

h4,
h5 {
    text-align: center;
}
</style>