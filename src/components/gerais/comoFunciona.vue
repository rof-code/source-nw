<template>
    <section id="comoFunciona">
		<div class="container">
			<div class="row">
				<div class="col-sm-6 videoComoFunciona">
					<iframe class="tamanhoheight" width="100%" height="280" src="https://www.youtube.com/embed/g2cAMHRtwro" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
				</div>
				<div class="col-sm-6 centralizar tirarPadding" style="padding: 0px 0px 0px 50px; margin-top: 25px;">
					<br class="mob"><br class="mob">
					<h1 class="titulosMob">
						<span style="color:#000000;">Entenda como funciona</span>
					</h1>
                    <br class="mob">
					<p class="subtituloMob" style=" font-size:20px; margin-top: -10px; line-height: 30px; font-weight:300;">
						Veja como é prático e fácil ter um sorriso <br>branquinho sem gastar muito.
					</p>
					<br>
					<div class="centralizar">
					<a href="/produtos" class="facaSeuPedido my-4">FAÇA SEU PEDIDO</a>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>



<style scoped>
#comoFunciona {
    padding: 50px 0px 50px 0px;
    background: #eeeeee !important; 
}

@media screen and (max-width:580px) {
    #comoFunciona{
        padding: 50px 0px 30px 0px !important;
    }
    .tirarPadding{
        padding: 0px !important;
        margin-top: 0px !important;
    }
    .centralizar{

        text-align: center !important;

    }
    .tamanhoheight{
        height: 100% !important;
    }
    .subtituloMob{
        padding:0px 10px;
        font-size: 18px !important;
    }
}

</style>