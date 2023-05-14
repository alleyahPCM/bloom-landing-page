<template>
    <div>
        <b-navbar toggleable="lg" type="light" variant="light" class="navbar-1">
            <b-navbar-brand href="#">
                    <img src="/img/bloom_logo.png" class="logo">
            </b-navbar-brand>

            <b-navbar-toggle target="nav-collapse" class="toggle-btn"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#"
                        ><span class="item-color">Customer</span></b-nav-item
                    >
                    <b-nav-item href="/sales"
                        ><span class="item-color">Sales</span></b-nav-item
                    >
                    <b-nav-item href="/customerservice" 
                        ><span class="item-color">Customer Service</span></b-nav-item
                    >
                    <b-nav-item href="/marketing-automation"
                        ><span class="item-color">Marketing Automation</span></b-nav-item
                    >
                    <b-nav-item href="/analytics"
                        ><span class="item-color">Analytics</span></b-nav-item
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
                        <b-button size="sm" class="my-2 my-sm-0 navbar-btn" type="submit"
                            >Search</b-button
                        >
                    </b-nav-form>

                    <b-nav-item-dropdown right>
                        <!-- Using 'button-content' slot -->
                        <template #button-content >
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
    div {
        font-family: 'Nunito', sans-serif;
    }

    .logo {
        width: auto;
        height: 50px;
        margin-right: 0 !important;
        margin-left: 15px;
    }

    
    .toggle-btn {
        margin-right: 15px;
    }

    .navbar-1{
        background-color: #3F4F34!important;
    }

    .navbar-btn {
        background-color: #86A760;
        border: none;
        color: #4D4114;
    }

    .navbar-btn:hover, .navbar-btn:active, .navbar-btn:focus{
        background-color: #739053 !important;
        color: #4D4114 !important;
    }
</style>

<script>
export default {
    name: "NavBar",
};
</script>
