<template lang="">
    <div class="see-why-container">
        <h2>
            See why over 500 organizations around the world use Greenfly
        </h2>
        <div>
            <div class="slide-1">slide-1</div>
            <div class="slide-2">slide-2</div>
            <div class="slide-3">slide-3</div>
            <div class="slide-4">slide-4</div>
        </div>
        <button type="button">Customer Success Stories</button>
    </div>
</template>
<script>
export default {

}
</script>

<style  scoped>
.see-why-container {
    background-color: #f2f2f2;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 3rem;
}

h2 {
    font-size: 2rem;
    font-weight: 700;
    margin: 0 auto;
    margin-bottom: 2rem;
    width: 40ch;
    text-align: center;
}

.see-why-container>div {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    width: 100%;
    margin: 0 auto;
    margin-bottom: 2rem;
}

button {
    background-color: white;
    padding: 1rem 1.5rem;
    border-color: var(--main-accent-color);
    outline: none;
    border-radius: 25px;
    color: var(--main-accent-color);
    font-weight: 700;
    cursor: pointer;
}
</style>