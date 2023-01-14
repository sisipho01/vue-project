<template>
    <section id="contact">
        <div class="container mt-3 contactContent">
            <h1 class="text-center">Contact Me</h1>

            <div class="row mt-4">
                <div class="col-lg-6">
                    <!-- to edit google map goto https://www.embed-map.com type your location, generate html code and copy the html  -->
                    <div
                        style="max-width:100%;list-style:none; transition: none;overflow:hidden;width:500px;height:500px;">
                        <div id="google-maps-display" style="height:100%; width:100%;max-width:100%;">
                            <iframe style="height:100%;width:100%;border:0;" frameborder="0"
                                src="https://www.google.com/maps/embed/v1/place?q=Langa,+Cape+Town,+South+Africa&key=AIzaSyBFw0Qbyq9zTFTd-tUY6dZWTgaQzuU17R8">
                            </iframe>
                        </div>
                        <a class="from-embedmap-code" rel="nofollow" href="https://www.bootstrapskins.com/themes"
                            id="grab-map-info">premium bootstrap themes</a>
                    </div>
                </div>

                <div class="col-lg-6">
                    <!-- form fields -->
                    <form action=https://formspree.io/f/xpznkzdw method="POST">
                        <input type="text" class="form-control form-control-lg" placeholder="Name">
                        <input type="email" class="form-control mt-3" placeholder="Email">
                        <input type="text" class="form-control mt-3" placeholder="Subject">
                        <div class="mb-3 mt-3">
                            <textarea class="form-control" rows="5" id="comment" name="text"
                                placeholder="Project Details"></textarea>
                        </div>

                        <button type="submit" class="btn btn-secondary mt-3">Contact Me</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

</template>
<script> 
export default{
    
}
</script>