<script>
export default {
    data() {
        return {
            listLinkComics: [
                { name: "Character", active: false, },
                { name: "Comics", active: false, },
                { name: "Movies", active: false, },
                { name: "TV", active: false, },
                { name: "GAMES", active: false, },
                { name: "Videos", active: false, },
                { name: "News", active: false, },
            ],
            listLinkShop: [
                { name: "Shop DC", active: false, },
                { name: "Shop DC Collectibles", active: false, },
            ],
            listLinkDc: [
                { name: "Terms Of Use", active: false, },
                { name: "Privacy policy (New)", active: false, },
                { name: "Ad Choices", active: false, },
                { name: "Advertising", active: false, },
                { name: "Jobs", active: false, },
                { name: "Subscriptions", active: false, },
                { name: "Talent Workshops", active: false, },
                { name: "CPSC Certificates", active: false, },
                { name: "Ratings", active: false, },
                { name: "Shop Help", active: false, },
                { name: "Contact Us", active: false, }
            ],
            listLinkSites: [
                { name: "DC", active: false, },
                { name: "MAD Magazine", active: false, },
                { name: "DC Kids", active: false, },
                { name: "DC Power Visa", active: false, },
            ],
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrap">
            <div class="list">
                <div class="block">
                    <p>DC COMICS</p>
                    <ul>
                        <li v-for="item in listLinkComics" :key="item.name"><span><a href="">{{ item.name }}</a></span></li>
                    </ul>

                    <p class="shop">SHOP</p>
                    <ul>
                        <li v-for="item in listLinkShop" :key="item.name"><span><a href="">{{ item.name }}</a></span></li>
                    </ul>
                </div>
            </div>

            <div class="list">
                <p>DC</p>
                <ul>
                    <li v-for="item in listLinkDc" :key="item.name"><span><a href="">{{ item.name }}</a></span></li>
                </ul>
            </div>

            <div class="list">
                <p>SITES</p>
                <ul>
                    <li v-for="item in listLinkSites" :key="item.name"><span><a href="">{{ item.name }}</a></span></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    height: 450px;
    color: white;
    display: flex;
    align-items: center;

    .wrap {
        display: flex;
        gap: 1.5rem;

        .shop {
            margin-top: 1.5rem;
        }

        p {
            margin-bottom: .4rem;
        }

        ul {
            color: grey;
            list-style: none;
        }

        li {
            margin-bottom: .2rem;

            a {
                color: inherit;
                text-decoration: none;
            }
        }
    }
}
</style>