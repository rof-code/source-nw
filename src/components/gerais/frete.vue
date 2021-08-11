<template>
    <div class="frete">
        <div class="container desk">
            <div class="row">
                <div class="col-sm-3 d-flex">
                    <div class="col-3">
                         <img src="@/assets/newwhite/badge.png" alt="">
                    </div>
                   <div class="col-9">
                    <p>COLÁGENO PREFERIDO</p>
                    <p>das celebridades</p>
                   </div>
                </div>
                <div class="col-sm-3 d-flex" style="">
                    <div class="col-3">
                         <img src="@/assets/newwhite/credit.png" alt="">
                    </div>
                    <div class="col-9" style="position:relative;right:-7%;">
                        <p>PAGUE COM CARTÃO</p>
                        <p>em até 12x sem juros</p>
                    </div>
                   
                </div>
                <div class="col-sm-3 d-flex" style="position:relative;right:-2%;">
                    <div class="col-3">
                          <img src="@/assets/newwhite/delivery.png" alt="">
                    </div>
                    <div class="col-9" style="position:relative;right:-9%;">
                        <p>FRETE GRÁTIS</p>
                        <p>para todo Brasil</p>
                    </div>
                 
                </div>
                <div class="col-sm-3 d-flex">
                    <div class="col-3">
                        <img src="@/assets/newwhite/lock.png" alt="">
                    </div>
                    <div class="col-9">
                        <p>SITE 100% SEGURO</p>
                        <p>com segurança SSL</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="container mob">
            <div class="row">
                <div class="col-6 text-center">
                    <img src="@/assets/newwhite/badge.png" alt="">
                    <p>COLÁGENO PREFERIDO</p>
                    <p>das celebridades</p>
                </div>
                <div class="col-6 text-center">
                    <img src="@/assets/newwhite/credit.png" alt="">
                    <p>PAGUE COM CARTÃO</p>
                    <p>em até 12x sem juros</p>
                </div>
            </div>
            <br>
            <div class="row">
                <div class="col-6 text-center">
                    <img src="@/assets/newwhite/delivery.png" alt="">
                    <p>FRETE GRÁTIS</p>
                    <p>para todo Brasil</p>
                </div>
                <div class="col-6 text-center">
                    <img src="@/assets/newwhite/lock.png" alt="">
                    <p>SITE 100% SEGURO</p>
                    <p>com segurança SSL</p>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .frete{
        background-color:#0046a0;
        padding:20px 0px;
        margin-top:-10px;
        .container.desk{
            .row{align-items: center; justify-content: center;}
            .col-sm-3.d-flex{
                align-items:center;
                p:first-child{
                    color: #fff;
                    font-size: 12px;
                    margin-bottom: 0;
                    font-weight: 800;
                }
                p:last-child{
                    color: #fff; 
                }
            }
        }
        .container.mob{
            .col-6{
                p:nth-last-of-type(2){
                    font-weight:bold;
                    font-size:13px;
                    margin-top:10px;
                    color:#fff;
                }
                p:nth-of-type(2){
                    color:#fff;
                }
                img{
                    margin:10px 0px;
                }
            }
        }
    }
</style>