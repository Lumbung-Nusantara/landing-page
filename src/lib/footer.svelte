<script>
    import { MapPinIcon, MailIcon, PhoneIcon, InstagramIcon, LinkedinIcon, YoutubeIcon, FacebookIcon} from 'svelte-feather-icons';
</script>

<div class="container px-5 pt-5">
    <div class="row mb-5">
        <div class="col-4 px-5">
            <img src="http://localhost:3000/assets/logo.png" alt="logo" class="logo mx-auto mb-4 d-block">
            <p>
                Lorem ipsum dolor amet cons adipisicing elit sed do 
                eiusmod tempor incididunt ut labore et dolore magna aliqua. 
                Ut enim ad minim veniam quis nostrud exercitation ullamco laboris nisi ut aliquip.
            </p>
        </div>
        <div class="col-4 px-5">
            <h4><b>Contact Info</b></h4>
            <ul class="px-0">
                <li class="my-3">
                    <MapPinIcon size={"1.2x"}/>
                    <span>Indonesia</span>
                </li>
                <li class="my-3">
                    <MailIcon size={"1.2x"}/>
                    <span>lumbungnusantara@gmail.com</span>
                </li>
                <li class="my-3">
                    <PhoneIcon size={"1.2x"}/>
                    <span>+62 123456789</span>
                </li>
            </ul>
        </div>
        <div class="col-4 px-5">
            <InstagramIcon class="mx-3"/>
            <LinkedinIcon class="mx-3"/>
            <YoutubeIcon class="mx-3"/>
            <FacebookIcon class="mx-3"/>
        </div>
    </div>
    <center class="py-2">
        <span>
            Copyright &copy; 2022 Lumbung Nusantara.
        </span>
    </center>
</div>

<style>
    .container{
        max-width: none;
        position: relative;
        background-color: #fab622cc;
    }

    .logo{
        max-width: 50%;
    }

    ul {
        list-style-type: none;
    }
</style>

<!-- <div class="footer-area pt-200" style="user-select: auto;">
    <div class="container" style="user-select: auto;">
        <div class="footer-bg pb-50" style="user-select: auto;">
            <div class="row" style="user-select: auto;">
                <div class="col-xl-3 col-lg-3 col-md-6" style="user-select: auto;">
                    <div class="footer-wrapper mb-30" style="user-select: auto;">
                        <div class="footer-logo" style="user-select: auto;">
                            <a href="index.html" style="user-select: auto;"><img src="img/logo/white.png" alt="" style="user-select: auto;"></a>
                        </div>
                        <div class="footer-text" style="user-select: auto;">
                            <p style="user-select: auto;">Lorem ipsum dolor amet cons adipisicing elit sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam quis nostrud exercitation ullamco laboris nisi ut aliquip.</p>
                        </div>
                        <div class="footer-icon" style="user-select: auto;">
                           <a href="/#" style="user-select: auto;"><i class="fab fa-facebook-f" style="user-select: auto;"></i></a>
                           <a href="/#" style="user-select: auto;"><i class="fab fa-twitter" style="user-select: auto;"></i></a>
                           <a href="/#" style="user-select: auto;"><i class="fab fa-linkedin" style="user-select: auto;"></i></a>
                           <a href="/#" style="user-select: auto;"><i class="fab fa-youtube" style="user-select: auto;"></i></a>
                           <a href="/#" style="user-select: auto;"><i class="fab fa-behance" style="user-select: auto;"></i></a>
                       </div>
                    </div>
                </div>
                <div class="col-xl-3 col-lg-3 col-md-6" style="user-select: auto;">
                    <div class="footer-wrapper pl-45 mb-30" style="user-select: auto;">
                        <div class="footer-title" style="user-select: auto;">
                            <h4 style="user-select: auto;">Customer Support</h4>
                            <img src="img/shape/f.png" alt="" style="user-select: auto;">
                        </div>
                        <ul class="fotter-menu" style="user-select: auto;">
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Help and Ordering</a></li>
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Privacy Policy</a></li>
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Return &amp; Cancellation</a></li>
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Delevery Schedule</a></li>
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Get a Call</a></li>
                            <li style="user-select: auto;"><a href="/#" style="user-select: auto;">Online Enquiry</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-xl-3 col-lg-3 col-md-6" style="user-select: auto;">
                    <div class="footer-wrapper pl-45 mb-30" style="user-select: auto;">
                        <div class="footer-title" style="user-select: auto;">
                            <h4 style="user-select: auto;">Contact Info</h4>
                            <img src="img/shape/f.png" alt="" style="user-select: auto;">
                        </div>
                        <ul class="fotter-link" style="user-select: auto;">
                            <li style="user-select: auto;"><i class="far fa-paper-plane" style="user-select: auto;"></i> <span style="user-select: auto;">205 Olazu Familia, Herba Street Front USA</span></li>
                            <li style="user-select: auto;"><i class="far fa-envelope-open" style="user-select: auto;"></i> <span style="user-select: auto;">zomatainfo@gmail.com</span></li>
                            <li style="user-select: auto;"><i class="fas fa-headphones" style="user-select: auto;"></i> <span style="user-select: auto;">002- 01008431112</span></li>
                        </ul>
                    </div>
                </div>
                <div class="col-xl-3 col-lg-3 col-md-6" style="user-select: auto;">
                    <div class="footer-wrapper pl-40 mb-30" style="user-select: auto;">
                        <div class="footer-title" style="user-select: auto;">
                            <h4 style="user-select: auto;">Newsletters</h4>
                            <img src="img/shape/f.png" alt="" style="user-select: auto;">
                        </div>
                        <div class="footer-content" style="user-select: auto;">
                            <p style="user-select: auto;">Enter your email and we’ll send you latest information plans.</p>
                        </div>
                        <div class="subscribes-form" style="user-select: auto;">
                            <form action="#" style="user-select: auto;">
                                <input placeholder="Enter your emaill " type="email" style="user-select: auto;">
                                <button class="btn" style="user-select: auto;">Subscribe</button>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom-area" style="user-select: auto;">
            <div class="row" style="user-select: auto;">
                <div class="col-xl-12" style="user-select: auto;">
                    <div class="copyright text-center" style="user-select: auto;">
                        <p style="user-select: auto;">Copyright <i class="far fa-copyright" style="user-select: auto;"></i> 2019 <a href="/#" style="user-select: auto;">BDevs</a>. All Rights Reserved</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div> -->
