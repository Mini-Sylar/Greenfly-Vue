<template lang="">
    <div class="see-why-container">
        <h2>
            See why over 500 organizations around the world use Greenfly
        </h2>
        <div class="slides-container">
            <div class="slide-1"><img src="@/assets/images/aecom.png" alt=""></div>
            <div class="slide-2"><img src="@/assets/images/ibm.png" alt=""></div>
            <div class="slide-3"><img src="@/assets/images/oracle.png" alt=""></div>
            <div class="slide-4"><img src="@/assets/images/uber.png" alt=""></div>
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
    border: 1px solid var(--main-accent-color);
    outline: none;
    border-radius: 25px;
    color: var(--main-accent-color);
    font-weight: 700;
    cursor: pointer;
}

.slides-container {
    width: 100%;
}

img {
    width: 50%;
    height: 100%;
    margin: 0 auto;
    object-fit: contain;
    display: flex;
    justify-content: center;
    align-items: center;
    filter: grayscale(100%);
    transition: .5s ease;
}

img:hover {
    filter: grayscale(0%);
}
</style>