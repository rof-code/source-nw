<template>
<footer>
	<news/>
	<section class="footer_links" style="background-color:#fafafb;padding:30px 0px;border-bottom:1px solid #ebebf3;">
		<div class="container">
			<div class="row justify-content-center">
				<div class="col-sm-3">
					<div class="col-sm-12 p-0">
						<p class="ajusteLeft" style="color:#404040;font-weight:bold;font-size:17px;">Nós enviamos e-mails incríveis</p>
						<p class="ajusteLeft" style="font-size:13px;text-align:left;">Saiba primeiro dos nossos lançamentos, <br class="mob"> coleções e
						promoções exclusivas.</p>
						<form class="formNews" action="https://news.mailclick.me/subscribe.php" method="post" accept-charset="UTF-8" target="blank" autocomplete="off" align="center;">
						<div class="row justify-content-center">
							<input type="email" id="newsletter" class="form-control" placeholder="Digite seu melhor e-mail" name="FormValue_Fields[EmailAddress]" control-id="ControlID-4" style="border-radius:0px !important;display:inline-block;">

							<input type="submit" class="btn btn-sub" name="FormButton_Subscribe" value="OK" id="FormButton_Subscribe" control-id="ControlID-5" style="display:inline;background-color:#0053B1 !important;color:#fff !important;padding:10px 15px 10px 10px !important;">
						</div>
						<input type="hidden" name="FormValue_ListID" value="6568" control-id="ControlID-6">
						<input type="hidden" name="FormValue_Command" value="Subscriber.Add" id="FormValue_Command">
						</form>
						<div class="row" style="padding-left:20px;margin-top:30px;">
						<a href="https://www.facebook.com/newwhitebr/" target="_blank">
							<img class="mx-2" src="@/assets/newwhite/FACEBOOK.png">
						</a>
						<a href="https://www.instagram.com/newwhitebr/" target="_blank">
							<img class="mx-2" src="@/assets/newwhite/INSTAGRAM.png">
						</a>
						</div>
					</div><!--col-sm-12-->
				</div><!--col-sm-3-->

				<div class="col-sm-2 colLinks">
					<div class="col-sm-12 links_r">
						<p style="color:#404040;font-weight:bold;font-size:17px;">Links Úteis</p>
						<a href="pagina/quem-somos">Quem Somos</a>
						<a href="pagina/atendimento">Atendimento</a>
						<a>Meus Pedidos</a>
						<a href="pagina/duvidas-frequentes">Perguntas Frequentes</a>
						<a href="pagina/politicas-de-privacidade">Políticas de Privacidade</a>
						<a href="pagina/tabela-nutricional">Tabela Nutricional</a>
						<a href="pagina/termos">Termos e Condições</a>
					</div>
				</div>

				<div class="col-sm-3">
					<div class="col-sm-12 colRelacionamento">
						<p style="color:#404040;font-weight:bold;font-size:17px;">Relacionamento</p> 
						<p style="font-size:16px;color:#666666;">Horário de atendimento: <br>
						Segunda a sexta-feira das <br>
						8h as 18h.</p>
						<a href="mailto:atendimento@vitabe.com.br" style="margin:10px 0px;color:#666666;">atendimento@vitabe.com.br</a>
						<a href="https://api.whatsapp.com/send?phone=5519998005679" target="_blank" style="display:inline-block;background-color:#0053B1;color:#fff;border-radius:6px;padding:10px;margin-top:20px;">CHAT ONLINE </a>
					</div>
				</div>

				<div class="col-sm-3">
					<div class="col-sm-12 colPagamentos">
						<p style="color:#404040;font-weight:bold;font-size:17px;">Formas de pagamento</p> 
						<img class="imgResponsive" src="@/assets/newwhite/PAYMENT.png">
					</div>
				</div>
			</div>
		</div>
	</section><!--links--->
	<section class="final_footer" style="background-color:#fafafb;padding: 20px 0px;">
		<div class="container">
			<div class="row">
				<div class="col-sm-8">
					<div class="col-sm-12">
						<p style="color:#000;font-size:16px;"><strong>Copyright © <span id="changeY"></span> New White. Todos os direitos reservados.</strong></p>
						<p style="color:#666666;font-size:14px;">
						Todo o conteúdo do site, todas as fotos, imagens, logotipos, marcas, layout, aqui veículados são de 
						propriedade exclusiva da Vita Be Comércio e Serviços LTDA. É vedada qualquer reprodução, total 
						ou parcial, de qualquer elemento de identidade, sem expressa autorização. A violação de qualquer 
						direito mencionado implicará na responsabilização cível e criminal nos termos da Lei.<br>
						<br>

						Rod. Governador Mario Covas, 882, Sala 24, Padre Mathias - Cariacica - ES, CEP: 29.157-100 - 
						CNPJ: 14.144.597/0002-33
						<br>
						<br>

						Os preços dos produtos estão sujeitos a alteração sem aviso prévio.</p>
					</div>
				</div>
			
				<div class="col-sm-4">
					<br class="mob"/>
					<div class="col-sm-12">
						<p style="color:#000;font-size:16px;"><strong>Certificados de Segurança</strong></p>
						<img class="imgResponsive" src="@/assets/newwhite/selos_rodape.png">
					</div>
				</div>
			</div><!--row-->
		</div><!--container-->
	</section>
</footer>
</template>

<script>
export default {
	mounted(){
		var dateFooter = new Date();
		var ano = dateFooter.getFullYear();
		var span = document.getElementById('changeY');
		span.textContent = ano.toString();
	},
	components:{
		news: () => import(`@/components/gerais/rodape/newsletter.vue`),
	}
}
</script>

<style scoped>
.mob{display:none;}
footer{
	padding:30px 0;
}
.footer_links input#newsletter{
	border-radius:none !important;
	width:70%;
	display:inline-block;
	padding-left:15px;
	height:45px;
}
.links_r{
	padding:0px;
}
.links_r a{
	font-size:16px;
	color:#666666;
	display:block;
}
@media screen and (max-width: 768px){
	.colLinks{
		padding-left:30px;
		margin-top:20px;
	}
	.ajusteLeft{
		padding-left:15px;
	}
	.colRelacionamento{
		margin-top:20px;
	}
	.colPagamentos{
		margin-top:20px;
	}
	.mob{display:block;}
}
</style>

