<template>
    <footer>
        <div class="cols">
            <img src="../assets/img/dc-logo-bg.png" alt="">
            <div>
                <h3>dc comics</h3>
                <nav>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                </nav>
                <h3>shop</h3>
                <nav>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </nav>
            </div>
            <div>
                <h3>dc</h3>
                <nav>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </nav>
            </div>
            <div>
                <h3>sites</h3>
                <nav>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="footer_social">
            <a class="button" href="">
                sign-up now!
            </a>
            <div class="social">
                <div class="follow_us">
                    follow us
                </div>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>

    .cols {
        position: relative;
        display: flex;
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 30px 10px;
    } 

    .cols > img {
        position: absolute;
        height: 300px;
        transform: translate(-50%, -50%);
        top: 50%;
        left: 70%;
        overflow: hidden;
    }

    .cols > div {
        margin-right: 30px;
    }

    h3 {
        text-transform: uppercase;
        color: white;
        padding: 10px 0;
    }

    ul {
        list-style: none;

        li {
            a {
                color: grey;
                font-size: 14px;
                text-decoration: none;
            }
        }
    }

    .footer_social {
        display: flex;
        height: 100px;
        background-color: #303030;
        align-items: center;
        justify-content: space-between;

        .button {
            margin: 10px;
            padding: 7px;
            border: 2px solid #256BF1;
            text-transform: uppercase;
            color: white;
            text-decoration: none;
        }

        .social {
            display: flex;
            align-items: center;
            .follow_us {
                text-transform: uppercase;
                color: #256BF1;
                margin: 10px;
                font-size: 18px;
                cursor: pointer;
            }
            img {
                margin: 10px;
                cursor: pointer;
            }
        }
    }
</style>