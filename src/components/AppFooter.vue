<template>
    <footer>
        <div class="inner-footer">
            <div class="column-1">
                <img src="../assets/logo.png" alt="logo" width="50" height="50">
                <p>Quadra QS 615 Bloco G 489 - Samambaia DF</p>
            </div>
            <div class="column-2">
                <img src="../assets/logo.png" alt="logo" width="50" height="50">
            </div>
            <div class="column-3">
                <p>Informations</p>
                <ul>
                    <li>
                        <a>placeholder</a>
                    </li>
                    <li>
                        <a>placeholder</a>
                    </li>
                    <li>
                        <a>placeholder</a>
                    </li>
                    <li>
                        <router-link to="/about">Something about us</router-link>
                    </li>
                </ul>
            </div>
            <div class="column-4">
                <p>Social media</p>
                <div class="sc-icon-holder">
                    <a>
                        <img src="../assets/logo.png" alt="logo" width="25" height="25">
                    </a>
                    <a>
                        <img src="../assets/logo.png" alt="logo" width="25" height="25">
                    </a>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>test store all rights reserved ©</p>
            <div class="hr"></div>
            <p>powered by coffee</p>
        </div>
    </footer>
</template>

<script>
export default {
    name: "AppFooter"
}
</script>

<style scoped>
footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: var(--primary);
    color: #fff;
    padding: 25px 15px;
    position: relative;
    top: 75px;
}

.inner-footer {
    display: grid;
    grid-gap: 125px;
    grid-template-columns: repeat(4, 1fr);
}

.inner-footer .column-1 img {
    display: block;
    margin-left: auto;
    margin-right: auto;
}

.inner-footer .column-1 p {
    margin-top: 10px;
    word-wrap: break-word;
    min-width: 140px;
    text-align: center;
}

.inner-footer .column-2 *{
    display: none;
}

.inner-footer .column-3 p {
    margin-bottom: 10px;
}

.inner-footer .column-3 ul li {
    padding: 7px 0;
}

.inner-footer .column-3 ul li * {
    color: white;
    text-decoration: none;
}

.inner-footer .column-4 p {
    margin-bottom: 10px;
}

.inner-footer .column-4 .sc-icon-holder a {
    margin: 10px 10px 10px 0;
    width: 25px;
    height: 25px;
}

.copyright {
    margin-top: 25px;
    text-transform: capitalize;
}

.copyright * {
    display: inline;
}

.copyright .hr {
    width: 0;
    border: 1px solid white;
    height: 14px;
    margin: 0 10px;
}

@media (max-width: 700px) {
    .inner-footer {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        grid-gap: 25px;
    }
}

</style>