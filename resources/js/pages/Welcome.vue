<template>
    <b-container fluid="sm" class="text-center welcome-container bv-example-row">
             <b-row class="landing-page-content">
                <b-row class="inner-row">
                    <h1>Welcome to Bloom</h1>
                    <br>
                    <p>It is a customer relationship management software. It could help businesses manage customer interactions
                        and improve customer satisfaction. May it be software, tools, and resources for your business. Beneficial
                        for early staged businesses which could attract customers and simplify business processes so owners could 
                        focus on the objectives of the business which is to increase the sales and revenue. That's Bloom.
                    </p>
                    <br>
                    <b-button class="landing-page-btn" href="/index">Get Started</b-button>
                </b-row>
            </b-row>
            <b-row class="footer">
                <div class="links">
                    <a href="#">Privacy Policy</a> 
                    <span> | </span>
                    <a href="#">Safe Guarding Statement</a> 
                    <span> | </span>
                    <a href="/about">About</a>
                    <span> | </span>
                    <a href="/contactUs">Contact Us</a>
                </div>

                <p id="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin sollicitudin, est quis porta consequat, sem nisi 
                    pulvinar lorem, at ornare lorem eros id sapien. Ut enim lacus, egestas eu egestas et, auctor eget libero. 
                    Quisque et urna velit. Maecenas est arcu, dapibus ut risus in, posuere tempus arcu.</p>
            </b-row>  
    </b-container>
</template>

<script>
    export default {
        name: "Welcome",
        mounted() {
            console.log("Welcome mounted.");
        },
    };
</script>

<style>
    body {
        height: 100vh;
        font-family: 'Nunito', sans-serif;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        overflow: scroll;
        overflow-x: hidden;
    }

    .welcome-container {
        background-image: url('/img/landing_page_bg.png');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        background-color: #3F4F34;
        min-width: 100%; 
        height: 100vh; 
        display: flex;
        flex-direction: column;
    }

    .footer {
        background-color: #86A760;
        bottom: 0;
        padding: 10px;
        flex:none;
        font-size: 16px;  
    }

    .footer a, .footer a:hover, .footer span {
        color: #4D4114;
        text-decoration: none;
        font-weight: bold;
    }

    .footer p {
        color: #4D4114;
    }
    
    .landing-page-content {
        display: flex;
        flex-grow: 1;
        align-items: center;
        justify-content: center;
    }

    .landing-page-content p {
        font-size: 16px;  
        color: #86A760;          
    }

    @font-face {
        font-family: StreuselKuchen-Regular;
        src: url('/fonts/StreuselKuchen-Regular.otf');
    }
    
    .landing-page-content h1 { 
        font-family: StreuselKuchen-Regular;
        font-size: 80px;
        color: #C88512;          
    }

    .inner-row {
        max-width: 600px; /* Set the desired width of the inner row */
        margin: 0 auto; /* Center the inner row horizontally */
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .landing-page-btn {
        width: 173px;
        border-radius: 11px;
        font-size: 20px;
        background-color: #86A760;
        border: none;
        color: #4D4114;
        margin-bottom: 40px;
    }

    .landing-page-btn:hover, .landing-page-btn:active, .landing-page-btn:focus{
        background-color: #739053 !important;
        color: #4D4114 !important;
    }
</style>


