<h1>Implementação Intro.JS (Tour) em HTML</h1>
<hr/>

```<!--INCLUIR Intro.js (CSS/JS) -->

<link rel="stylesheet" href="introjs.min.css">
<script src="introjs.min.js">

<!-- INICIALIZAR AUTOMATICAMENTE (Função pode ser chamada no click ou outros eventos) -->
<script>
    introJs().start();
</script>

<!-- NOS ELEMENTOS HTML DA PÁGINA, DEFINIR
STEP | INTRO
EXEMPLO: /templates/dashboard/details.html: -->

<div class="card-footer">
	<div class="botoes-bemvindo">
		<!-- PASSO 1 -->
		<a data-step="1" data-intro="Novo visual para criação de produtos. Clique no botão acima para iniciar o cadastro de produtos de seu estabelecimento Cardapex."  href="{% url 'dashboard:products:list' tenant.uuid %}" class="btn btn-primary btn-md"><i class="fas fa-utensils mr-1"></i> Criar um Produto</a>
		<!-- PASSO 2 -->
		<a data-step="2" data-intro="Adicione seus produtos à categorias. Com o cadastro de categorias você consegue organizar seus produtos de forma intuitiva para o consumidor final." href="{% url 'dashboard:categories:list' tenant.uuid %}" class="btn btn-primary btn-md"><i class="fas fa-list mr-1"></i> Criar uma Categoria</a>
	</div>
</div>
```

