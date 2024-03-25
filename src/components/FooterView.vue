<template>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <footer>
        <div class="container">
            <div class="footer-top">
                <div class="row">
                    <div class="col-md-6 col-lg-3 about-footer">
                        <h3> <span class="L">M</span>ATTHEW <span class="A">S</span>WAIN </h3>
                        <ul>
                            <li><i class="fa fa-phone" aria-hidden="true"></i>
                                +27 79 318 2409 <br> +27 21 123 4567</li>
                        </ul>
                    </div>
                    <div class="col-md-6 col-lg-2 page-more-info">
                        <div class="footer-title">
                            <h4>Page links</h4>
                        </div>
                        <ul>
                            <li><i class="fa fa-home" aria-hidden="true"></i> -Home</li>
                            <li><i class="fa fa-user-secret" aria-hidden="true"></i> -About</li>
                            <li><i class="fa fa-phone" aria-hidden="true"></i> -Contact</li>
                        </ul>
                    </div>

                    <div class="col-md-6 col-lg-3 page-more-info">
                        <div class="footer-title">
                            <h4>More Info</h4>
                        </div>
                        <ul>
                            <li>Agent Requests Enquiries</li>
                            <li>Customer Care Relations</li>
                        </ul>
                    </div>
                    <div class="col-md-6 col-lg-4 open-hours">
                        <div class="footer-title">
                            <h4>Social Media</h4>
                        </div>
                            <ul class="footer-social">
                                <i class="fa fa-facebook" aria-hidden="true"></i>
                                <i class="fa fa-instagram" aria-hidden="true"></i>
                                <i class="fa fa-linkedin" aria-hidden="true"></i>
                                <i class="fa fa-whatsapp" aria-hidden="true"></i>
                            </ul>
                        <table class="table">
                        </table>
                    </div>
                </div>
            </div>
            <hr>
        </div>
            <div class="footer-bottom">
                <div class="row">
                    <div class="col-sm-8">
                        <p class="lead"> MATTHEW SWAIN - PORTFOLIO  &copy; <span>{{ currYear }}</span> </p>
                    </div>
                </div>
            </div>
    </footer>
</template>

<script>
export default {

    data() {
        return {
            currYear: new Date().getFullYear()
        }
    }
}
</script>

<style>
a,
a:active,
a:focus {
    color: #ddd;
    text-decoration: none;
    transition-timing-function: ease-in-out;
    -ms-transition-timing-function: ease-in-out;
    -moz-transition-timing-function: ease-in-out;
    -webkit-transition-timing-function: ease-in-out;
    -o-transition-timing-function: ease-in-out;
    transition-duration: .2s;
    -ms-transition-duration: .2s;
    -moz-transition-duration: .2s;
    -webkit-transition-duration: .2s;
    -o-transition-duration: .2s;
}

.L,
.A {
    color: gold;
}

ul {
    margin: 0;
    padding: 0;
    list-style: none;
    font-family: "Playfair Display", serif;

}

/*---------footer---------*/

footer {
    background-color: #000;
    background-image: linear-gradient(to bottom, #000, #111, #222, #333);
    color: #fff;
    padding: 50px;
    font-size: 17px;
    font-family: "Playfair Display", serif;
}

footer h3 {
    font-size: 24px;
    font-weight: 600;
    letter-spacing: 5px;
    font-family: "Playfair Display", serif;

}

footer h4 {
    font-size: 20px;
    font-weight: 600;
    letter-spacing: 1px;
    display: inline-block;
    margin-bottom: 2px;
}

.about-footer li i {
    position: absolute;
    left: 0;
}

.about-footer li {
    padding-left: 40px;
    position: relative;
    margin-bottom: 40px;
}

.about-footer ul {
    margin-top: 30px;
}

footer a {
    color: #fff;
}

footer a:hover {
    color: gold;
}

.footer-title {
    border-bottom: 2px solid gold;
    padding-bottom: 25px;
    margin-bottom: 35px;
}

ul.footer-social li {
    display: inline;
    margin-right: 16px;
}

ul.footer-social i {
    width: 30px;
    height: 30px;
    background: #fff;
    color: #000;
    text-align: center;
    line-height: 30px;
    border-radius: 30px;
    font-size: 16px;
    -webkit-transition: all 0.5s;
    -moz-transition: all 0.5s;
    -o-transition: all 0.5s;
    transition: all 0.5s;
    font-weight: 800;
}

ul.footer-social li:last-child {
    margin-right: 0px;
}

ul.footer-social i:hover {
    background: gold;
    color: #000;
}

.page-more-info li {
    margin-bottom: 10px;
}


footer .table td {
    position: relative;
    background-color: #ddd;
    font-weight: bold;
    padding: 7px;
}
.footer-bottom p {
    text-align: right;
}

.footer-bottom {
    margin-top: 30px;
}

.lead {
    color: #ddd;
}
</style>