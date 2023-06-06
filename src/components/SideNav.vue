<template>
    <div class="nav">
        <ul>
            <li class="">
                <button type="button" name="button" class="btn">Presentation</button>
            </li>
            <li class="">
                <button type="button" name="button" class="btn">Personnages</button>
            </li>
            <li class="">
                <button type="button" name="button" class="btn">Concept</button>
            </li>
            <li class="">
                <button type="button" name="button" class="btn">Produits derives</button>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    name: "side-nav",
};
</script>
<style scoped>
.nav {
    font-size: 1.6rem;
    line-height: 1.25rem;
    visibility: inherit;
    box-sizing: border-box;
    margin: 0;
    align-items: flex-start;
    display: flex;
    flex-direction: column;
    /* height: 100%; */
    justify-content: center;
    left: 1%;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    /* width: 100%; */
    color: #fffff7;
    position: fixed;
    z-index: 100000;
}
ul {
    font-size: 1.6rem;
    line-height: 1.25rem;
    visibility: inherit;
    color: #0b6b37;
    box-sizing: border-box;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
    list-style: none;
    padding-left: 1.625rem;
    position: relative;
}

ul:before {
    border-bottom: 1px solid;
    border-bottom-left-radius: 80px;
    border-left: 1px solid;
    border-top: 1px solid;
    border-top-left-radius: 80px;
    content: "";
    display: inline-block;
    height: calc(100% - 0.875rem);
    left: 0;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 16px;
}

li {
    font-size: 1.6rem;
    line-height: 1.25rem;
    visibility: inherit;
    color: #0b6b37;
    list-style: none;
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
    box-sizing: border-box;
    align-items: center;
    display: flex;
    margin: 0;
    position: relative;
    font-weight: 800;
}

li:not(:first-of-type):not(:last-of-type):before{
    background: currentColor;
    content: "";
    display: inline-block;
    height: 1px;
    left: -0.3125rem;
    position: absolute;
    top: 50%;
    transform: translate(-100%);
    width: 1.3125rem;
}

button {
    visibility: inherit;
    list-style: none;
    box-sizing: border-box;
    margin: 0;
    overflow: visible;
    all: unset;
    color: currentColor;
    cursor: pointer;
    pointer-events: auto;
    font-size: 0.4rem;
    position: relative;
    text-transform: uppercase;
}
</style>
