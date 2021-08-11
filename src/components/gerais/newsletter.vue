<template>
    <section class="newsletter">
        <div class="newsletterDesk desk">
            <div class="container">
                <div class="row">
                    <div class="col-sm-6 d-flex" style="position:relative;left:-5%;">
                        <div class="col-2">
                            <img src="@/assets/newwhite/ico22.png" alt="">
                        </div>
                        <div class="col-10">
                            <p
                            style="font-size:16px;color:#404040;font-weight:bold;"
                            >Nós enviamos e-mails incríveis</p>
                            <p 
                            style="font-size:12px;colorl:#888888;"
                            >Saiba primeiro dos nossos lançamentos, dicas e promoções exclusivas</p>
                        </div>
                    </div><!--col-sm-6-->
                    
                    <div class="col-sm-6 text-right">
                        <form class="formNews" action="https://news.mailclick.me/subscribe.php" method="post" accept-charset="UTF-8" target="blank" autocomplete="off">

                        <input style="width:75%; font-family: 'myriad-pro', sans-serif !important; color: #b7b7b7 !important; font-size:12px; padding-left:20px; display:inline-block; border-radius:20px; border:0px;" type="text" id="newsletter" class="form-control" placeholder="Digite seu melhor e-mail" name="FormValue_Fields[EmailAddress]" value="" required="" control-id="ControlID-1">

                        <input type="submit" style="display:inline-block; opacity: 100 !important; width:20%; padding:10px 0px 12px 0px; margin-left:-35px; border-radius:20px;font-weight:bold; background:#f13787; color:#fff; font-size:12px;" class="btn btn-sub" name="FormButton_Subscribe" value="Participar" id="FormButton_Subscribe" control-id="ControlID-2">

                        <input type="hidden" name="FormValue_ListID" value="6568" control-id="ControlID-3">
                        <input type="hidden" name="FormValue_Command" value="Subscriber.Add" id="FormValue_Command">

                        </form>
                    </div><!--col-sm-6-->
                </div>
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
.newsletterDesk{
    background-color:#e5e5e5;
    padding:20px 0px;
}
</style>