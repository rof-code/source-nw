<template>
    <div class="anime">
	<section id="Passos" class="desk" style="padding: 30px 0px 30px 0px;">
		<div class="container">
			<div class="row">
				<div class="col-sm-6 centralizarTexto" style="margin-top: 25px;" >
					<h1 class="titulosMob" style="color: #fff !important;">
						<span>Rápido e Prático</span><br><span> New White é assim</span>
					</h1>
					<p class="subtituloMob" style="margin-top:-10px; font-size:18px; line-height: 30px; color: #fff !important; font-weight:300;">
						Use ao acordar e antes de <br class="mob"> dormir durante 14 dias. <br class="desk">Depois é só usar 1 ou 2 vezes por semana <br class="desk">para manter seus dentes brancos!
					</p>
					<br><br>
					<div class="desk" style="width:20%;">
                        <a href="/produtos" class="facaSeuPedido my-4">FAÇA SEU PEDIDO</a>
					</div>

				</div>

				<div class="col-sm-6 imgPassos" style="text-align: right;">
					<img class="responsiveImg" style="width: 80%;" src="@/assets/newwhite/img-como-usar.png">
				</div>

				<div class="centralizarTexto mob col">
					<br class="mob"><br class="mob"><br class="mob">
					<div class="row justify-content-center"><a href="/produtos" class="facaSeuPedido my-4">FAÇA SEU PEDIDO</a></div>
					<br class="mob">
				</div>
			</div>
		</div>
	</section>


    <section class="rapidomob mob">
    <div class="pratico">
        <div class="container" style="margin-top:40px;">
            <div class="pratico_head">
                <h3>Rápido e prático, <br>
                    New White é assim
                </h3>
                <p style="text-align:left; color:#fff; font-size:16px;">Use ao acordar e antes de dormir durante 14<br>
                    dias. Depois é só usar 1 ou 2 vezes por semana para manter seus dentes<br>
                    branquinhos!
                </p>
                <br>
                <div class="buttonForm" style="width:20%;">
                      <a href="/produtos" class="facaSeuPedido my-4">FAÇA SEU PEDIDO</a>
                </div>
            </div>
        </div>
    </div>
    <div class="glider-contain mob" style="margin:20px 0px 0px 0px;padding: 30px 0px 30px 0px;">
      <div class="glider draggable">
      <div class="glider-track" style="width: 288px;"><div class="glider-slide active left-2 visible" data-gslide="0" style="height: auto; width: 72px;"><img src="@/assets/newwhite/01.png" alt="">
            <p>
                Com sua escova macia <br class="mob">
                úmida, mergulhe as <br class="mob">
                cerdas no pó.
            </p>
        </div><div class="glider-slide left-1 visible" data-gslide="1" style="height: auto; width: 72px;"><img src="@/assets/newwhite/02.png" alt="">
            <p>
                Escove gentilmente<br class="mob">
                por 3 minutos.
            </p>
        </div><div class="glider-slide center visible" data-gslide="2" style="height: auto; width: 72px;"><img src="@/assets/newwhite/03.png" alt="">
            <p id="centralizar3">
                Enxágue a boca <br class="mob">
                com água.
            </p>        
        </div><div class="glider-slide right-1 visible" data-gslide="3" style="height: auto; width: 72px;"><img src="@/assets/newwhite/04.png" alt="">
            <p>
                Escove com seu<br class="mob"> 
                creme dental.
            </p>        
        </div></div></div>
    </div>
    </section>
    </div>
</template>




<style scoped>
	#Passos {
		background-image:  url('../../assets/newwhite/fundoAzul.jpg');
		background-position: center top;
		background-repeat: no-repeat;
		background-size: 100% 470px;
	}

	@media screen and (max-width: 580px){
		#Passos {
			background-color: #2d4f98 !important;
			background-image: url();
		}

		#Passos img {
			width: 100%;
			background-color: #fff;
			padding: 10px;
			border-radius: 10px;
			margin-top: 40px;
		}
		.tirarTopo{
			margin-top: 0px !important;
		}

		.imgPassos{
			margin-top: -50px !important;
			text-align: center !important;
		}

		.responsiveImg{
			width: 100% !important;
		}

		.centralizarTexto{
			text-align: center !important;
		}

	}


    /* MOB */
    .glider, .glider-contain {
    margin: 0 auto;
    position:relative
}
.pratico{
    background-image: url("../../assets/newwhite/svgpratico.svg");
    background-size:cover;
    background-position:center;
    height:500px;
    padding:20px 0;
}
.pratico h3{
    font-size:36px;
    color:#fff;
}
.pratico p{
    font-size:18px;
}
#centralizar3{
    position:relative;
    right:-45px;
}
.rapidomob p{
    text-align:center;
    margin-top:20px;
    font-size:16px;
    font-weight:500;
}

.glider, .glider-track {
    transform:translateZ(0)
}

.glider-dot, .glider-next, .glider-prev {
    border: 0;
    padding: 0;
    user-select: none;
    outline:0
}

.glider-contain {
    width:100%
}

.glider {
    overflow-y: hidden;
    -webkit-overflow-scrolling: touch;
    -ms-overflow-style:none
}

.glider-track {
    width: 100%;
    margin: 0;
    padding: 0;
    display: flex;
    z-index:1
}

.glider.draggable {
    user-select: none;
    cursor: -webkit-grab;
    cursor:grab;
}
.glider.draggable .glider-slide img {
    user-select: none;
    pointer-events:none
}

.glider.drag {
    cursor: -webkit-grabbing;
    cursor:grabbing
}

.glider-slide {
    user-select: none;
    justify-content: center;
    align-content: center;
    width: 100%;
    min-width:180px;
    margin:0px 25px 0px 25px;
}

.glider-slide img {
    width:100%
}

.glider::-webkit-scrollbar {
    opacity: 0;
    height:0
}

.glider-next, .glider-prev {
    position: absolute;
    background: 0 0;
    z-index: 2;
    font-size: 40px;
    text-decoration: none;
    left: -23px;
    top: 30%;
    cursor: pointer;
    color: #666;
    opacity: 1;
    line-height: 1;
    transition:opacity .5s cubic-bezier(.17, .67, .83, .67), color .5s cubic-bezier(.17, .67, .83, .67)
}

.glider-next:focus, .glider-next:hover, .glider-prev:focus, .glider-prev:hover {
    color:#ccc
}

.glider-next {
    right: -23px;
    left:auto
}

.glider-next.disabled, .glider-prev.disabled {
    opacity: .25;
    color: #666;
    cursor:default
}

.glider-hide {
    opacity:0
}

.glider-dots {
    user-select: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 auto;
    padding:0
}

.glider-dot {
    display: block;
    cursor: pointer;
    color: #ccc;
    border-radius: 999px;
    background: #ccc;
    width: 12px;
    height: 12px;
    margin:7px
}

.glider-dot:focus, .glider-dot:hover {
    background:#ddd
}

.glider-dot.active {
    background:#a89cc8
}

@media (max-width: 36em) {
    .glider::-webkit-scrollbar {
        opacity: 1;
        -webkit-appearance: none;
        width: 7px;
        height:3px
    }

    .glider::-webkit-scrollbar-thumb {
        opacity: 1;
        border-radius: 99px;
        background-color: rgba(156, 156, 156, .25);
        -webkit-box-shadow: 0 0 1px rgba(255, 255, 255, .25);
        box-shadow: 0 0 1px rgba(255, 255, 255, .25)
    }
}

    /* MOB */
</style>