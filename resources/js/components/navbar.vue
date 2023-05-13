<template>
    <div>
        <b-navbar toggleable="lg" type="light" variant="light">
            <b-navbar-brand href="#">
                    <img src="/img/bloom_logo.png" class="logo">
            </b-navbar-brand>

            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#" class="border-left"
                        >Customer</b-nav-item
                    >
                    <b-nav-item href="/sales" class="border-left"
                        >Sales</b-nav-item
                    >
                    <b-nav-item href="/customerservice" class="border-left"
                        >Customer Service</b-nav-item
                    >
                    <b-nav-item href="/marketing-automation" class="border-left"
                        >Marketing Automation</b-nav-item
                    >
                    <b-nav-item href="/analytics" class="border-left"
                        >Analytics</b-nav-item
                    >
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="ml-auto">
                    <b-nav-form>
                        <b-form-input
                            size="sm"
                            class="mr-sm-2"
                            placeholder="Search"
                        ></b-form-input>
                        <b-button size="sm" class="my-2 my-sm-0" type="submit"
                            >Search</b-button
                        >
                    </b-nav-form>

                    <b-nav-item-dropdown right>
                        <!-- Using 'button-content' slot -->
                        <template #button-content>
                            <em>User</em>
                        </template>
                        <b-dropdown-item href="#">Profile</b-dropdown-item>
                        <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                    </b-nav-item-dropdown>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>

<style scoped>
    .logo {
        width: auto;
        height: 80px;
        margin-right: 0 !important;
    }
</style>

<script>
export default {
    name: "NavBar",
};
</script>
