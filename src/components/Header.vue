<template>
    <header class="header">
        <div class="logoWrapper">
            <a href="#" class="logoLink">
                <img src="./../../src/assets/decorations/logo.png" class="logoImage" alt="logoImage">
            </a>
        </div>

        <nav class="navigationMenu">
            <ul class="Menu">
                <li class="menuItems">
                    <a href="#" class="menuLinks">Home</a>
                </li>
                <li class="menuItems">
                    <a href="#" class="menuLinks">Introduction</a>
                </li>
                <li class="menuItems">
                    <a href="#" class="menuLinks">About</a>
                </li>
                <li class="menuItems">
                    <a href="#" class="menuLinks">Reviews</a>
                </li>
                <li class="menuItems">
                    <a href="#" class="menuLinks menuLinks--moreWidth">Latest Update</a>
                </li>
                <li class="menuItems">
                    <a href="#" class="menuLinks">Credits</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@import './../assets/scss/variables';
@import './../assets/scss/mixins';

.header {
    padding: 0 30px;
    width: 100%;
    height: 60px;
    background: transparent;
    border-bottom: 1px solid rgba(255, 255, 255, 0.25);
    position: fixed;
    @include rowLayout(space-between, center, 0);

    .logoWrapper {
        width: 160px;
        height: 100%;

        .logoLink {
            width: 100%;
            height: 100%;

            .logoImage {
                width: 100%;
                height: 100%;
            }
        }
    }

    .navigationMenu {
        width: 570px;
        height: 100%;

        .Menu {
            height: 100%;
            @include rowLayout(justify-content, center, 0);

            .menuItems {
                flex: 1;
                height: 100%;
                border-left: 0.8px solid rgb(43, 43, 43);

                .menuLinks {
                    color: #fff;
                    padding: 0 13px;
                    height: 100%;
                    font-size: 13px;
                    font-family: $primary-font-family ;
                    font-weight: 600;
                    @include rowLayout();

                    &--moreWidth {
                        width: 109px;
                    }
                }
            }
        }
    }
}
</style>


<script>
export default {

}
</script>