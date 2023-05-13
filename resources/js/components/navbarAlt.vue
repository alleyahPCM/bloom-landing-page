<template>
    <div>
        <b-navbar toggleable="lg" type="light" variant="light">
            <b-navbar-brand href="#">BLOOM</b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#" class="border-left"
                        >About us</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Contact us</b-nav-item
                    >
                    <b-nav-item href="#" class="border-left"
                        >Our work</b-nav-item
                    >
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">
                    <b-nav-form>
                        <b-button size="sm" class="my-2 my-sm-0">BLOOM</b-button>
                    </b-nav-form>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>

<style scoped></style>

<script>
export default {
    name: "NavBar",
};
</script>
