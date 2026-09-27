# assadinhos-da-lauri
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Assadinhos da Lauri</title>
<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,sans-serif;
    scroll-behavior:smooth;
}
body{
    background:#fff8ef;
    color:#2b170b;
}
/* TOPO */
header{
    position:sticky;
    top:0;
    z-index:100;
    background:#ff6b00;
    padding:18px 7%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    box-shadow:0 3px 15px #0002;
}
.logo{
    font-size:24px;
    font-weight:bold;
    color:white;
}
.logo span{
    color:#ffe1b3;
}
nav{
    display:flex;
    gap:20px;
}
nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}
/* HERO */
.hero{
    min-height:75vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:50px 20px;
    background:
    linear-gradient(#0008,#0008),
    url("https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=1400&q=80");
    background-size:cover;
    background-position:center;
}
.hero-content{
    max-width:750px;
    color:white;
}
.hero h1{
    font-size:clamp(42px,8vw,75px);
    margin-bottom:20px;
}
.hero p{
    font-size:20px;
    margin-bottom:15px;
}
.destaque{
    display:inline-block;
    background:#ff6b00;
    padding:10px 18px;
    border-radius:30px;
    font-weight:bold;
    margin-bottom:25px;
}
.entrega{
    color:#ffd28f;
    font-weight:bold;
    margin-bottom:30px;
}
.botao{
    display:inline-block;
    background:#ff6b00;
    color:white;
    padding:16px 30px;
    border-radius:10px;
    text-decoration:none;
    font-weight:bold;
    border:none;
    cursor:pointer;
    transition:.3s;
}
.botao:hover{
    transform:scale(1.05);
    background:#e85f00;
}
/* SEÇÕES */
section{
    padding:80px 7%;
}
.titulo{
    text-align:center;
    margin-bottom:45px;
}
.titulo h2{
    font-size:38px;
    color:#e65f00;
}
.titulo p{
    margin-top:10px;
    color:#795548;
}
/* CARDÁPIO */
.cardapio{
    display:grid;
    grid-template-columns:
    repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}
.item{
    background:white;
    border-radius:18px;
    overflow:hidden;
    box-shadow:0 5px 20px #0001;
    transition:.3s;
}
.item:hover{
    transform:translateY(-7px);
}
.item-img{
    height:180px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:75px;
    background:#fff0df;
}
.item-info{
    padding:22px;
}
.item h3{
    font-size:23px;
    margin-bottom:10px;
}
.item p{
    color:#795548;
    line-height:1.5;
}
.preco{
    display:block;
    margin-top:15px;
    font-size:23px;
    font-weight:bold;
    color:#e65f00;
}
/* CONTADOR */
.contador{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:15px;
    margin-top:20px;
}
.contador button{
    width:42px;
    height:42px;
    border:none;
    border-radius:50%;
    background:#ff6b00;
    color:white;
    font-size:25px;
    font-weight:bold;
    cursor:pointer;
}
.contador button:hover{
    background:#e85f00;
}
.quantidade{
    font-size:22px;
    font-weight:bold;
    min-width:30px;
    text-align:center;
}
/* PEDIDO */
.pedido{
    max-width:650px;
    margin:50px auto 0;
    background:white;
    padding:30px;
    border-radius:20px;
    box-shadow:0 5px 20px #0001;
}
.pedido h3{
    text-align:center;
    color:#e65f00;
    font-size:28px;
    margin-bottom:25px;
}
.resumo{
    border-top:1px solid #eee;
    border-bottom:1px solid #eee;
    padding:15px 0;
    margin-bottom:20px;
}
.linha{
    display:flex;
    justify-content:space-between;
    padding:7px 0;
    color:#60483c;
}
.total{
    display:flex;
    justify-content:space-between;
    font-size:24px;
    font-weight:bold;
    margin-bottom:25px;
}
/* FORMULÁRIO */
.formulario{
    margin-top:25px;
}
.formulario label{
    display:block;
    font-weight:bold;
    margin:15px 0 7px;
}
.formulario input,
.formulario textarea{
    width:100%;
    padding:14px;
    border:1px solid #ddd;
    border-radius:10px;
    font-size:16px;
    outline:none;
}
.formulario input:focus,
.formulario textarea:focus{
    border-color:#ff6b00;
}
.formulario textarea{
    min-height:90px;
    resize:vertical;
}
.whatsapp{
    width:100%;
    background:#25D366;
    text-align:center;
    margin-top:20px;
}
.whatsapp:hover{
    background:#1ebc59;
}
.aviso{
    text-align:center;
    color:#888;
    margin-top:12px;
    font-size:14px;
}
/* INFORMAÇÕES */
.info{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:20px;
}
.info div{
    background:white;
    padding:25px;
    border-radius:15px;
    min-width:230px;
    text-align:center;
    box-shadow:0 5px 15px #0001;
}
.info h3{
    color:#e65f00;
    margin-bottom:10px;
}
.info p{
    color:#60483c;
}
/* RODAPÉ */
footer{
    background:#180c06;
    color:#aaa;
    text-align:center;
    padding:25px;
}
/* CELULAR */
@media(max-width:650px){
    header{
        flex-direction:column;
        gap:12px;
    }
    nav{
        gap:12px;
    }
    nav a{
        font-size:14px;
    }
    section{
        padding:60px 5%;
    }
    .pedido{
        margin-left:5%;
        margin-right:5%;
    }
}
</style>
</head>
<body>
<header>
<div class="logo">
🍔 Assadinhos <span>da Lauri</span>
</div>
<nav>
<a href="#inicio">Início</a>
<a href="#cardapio">Cardápio</a>
<a href="#pedido">Pedido</a>
</nav>
</header>
<!-- INÍCIO -->
<section class="hero" id="inicio">
<div class="hero-content">
<h1>Assadinhos da Lauri</h1>
<p>
🍔 Lanches assados, feitos com carinho ❤️
</p>
<div class="destaque">
🔥 ESPECIALIDADE: LANCHES ASSADOS
</div>
<div class="entrega">
🛵 SOMENTE ENTREGA • A PARTIR DAS 14:00
</div>
<a href="#cardapio" class="botao">
🍔 Fazer pedido
</a>
</div>
</section>
<!-- CARDÁPIO -->
<section id="cardapio">
<div class="titulo">
<h2>🍔 Cardápio</h2>
<p>
Nossos lanches são assados e preparados com muito carinho!
</p>
</div>
<div class="cardapio">
<!-- HAMBÚRGUER -->
<div class="item">
<div class="item-img">
🍔
</div>
<div class="item-info">
<h3>Hambúrguer</h3>
<p>
Lanche assado, preparado
com carinho e muito sabor.
</p>
<span class="preco">
R$ 10,00
</span>
<div class="contador">
<button onclick="alterarQuantidade(0,-1)">−</button>
<span class="quantidade" id="qtd0">0</span>
<button onclick="alterarQuantidade(0,1)">+</button>
</div>
</div>
</div>
<!-- X-BACON -->
<div class="item">
<div class="item-img">
🥓🍔
</div>
<div class="item-info">
<h3>X-Bacon</h3>
<p>
Lanche assado com bacon
e ingredientes especiais.
</p>
<span class="preco">
R$ 15,00
</span>
<div class="contador">
<button onclick="alterarQuantidade(1,-1)">−</button>
<span class="quantidade" id="qtd1">0</span>
<button onclick="alterarQuantidade(1,1)">+</button>
</div>
</div>
</div>
<!-- X-BACON CHEDDAR -->
<div class="item">
<div class="item-img">
🧀🥓🍔
</div>
<div class="item-info">
<h3>X-Bacon / Cheddar</h3>
<p>
Lanche assado com bacon,
cheddar e muito sabor.
</p>
<span class="preco">
R$ 15,00
</span>
<div class="contador">
<button onclick="alterarQuantidade(2,-1)">−</button>
<span class="quantidade" id="qtd2">0</span>
<button onclick="alterarQuantidade(2,1)">+</button>
</div>
</div>
</div>
</div>
<!-- PEDIDO -->
<div class="pedido" id="pedido">
<h3>🛒 Seu Pedido</h3>
<div class="resumo" id="resumo">
<p style="text-align:center;color:#888;">
Nenhum lanche selecionado.
</p>
</div>
<div class="total">
<span>Total:</span>
<span id="total">
R$ 0,00
</span>
</div>
<!-- DADOS DO CLIENTE -->
<div class="formulario">
<label for="nome">
👤 Seu nome
</label>
<input
type="text"
id="nome"
placeholder="Digite seu nome">
<label for="endereco">
📍 Endereço para entrega
</label>
<textarea
id="endereco"
placeholder="Rua, número, bairro e complemento"></textarea>
<label for="observacao">
📝 Observação (opcional)
</label>
<textarea
id="observacao"
placeholder="Ex.: tirar algum ingrediente, ponto de referência..."></textarea>
</div>
<a
class="botao whatsapp"
href="#"
onclick="enviarPedido(event)">
💬 Enviar pedido pelo WhatsApp
</a>
<p class="aviso">
🛵 Somente entrega • Pedidos a partir das 14:00
</p>
</div>
</section>
<!-- INFORMAÇÕES -->
<section>
<div class="titulo">
<h2>📋 Informações</h2>
</div>
<div class="info">
<div>
<h3>🔥 Lanches</h3>
<p>
Todos os nossos lanches são assados.
</p>
</div>
<div>
<h3>🛵 Entrega</h3>
<p>
Somente delivery.
</p>
</div>
<div>
<h3>⏰ Horário</h3>
<p>
A partir das 14:00.
</p>
</div>
</div>
</section>
<footer>
© 2026 Assadinhos da Lauri ❤️
<br>
Lanches assados feitos com carinho.
</footer>
<script>
const produtos = [
{
    nome:"Hambúrguer",
    preco:10
},
{
    nome:"X-Bacon",
    preco:15
},
{
    nome:"X-Bacon / Cheddar",
    preco:15
}
];
let quantidades = [0,0,0];
function alterarQuantidade(index,valor){
    quantidades[index] += valor;
    if(quantidades[index] < 0){
        quantidades[index] = 0;
    }
    document.getElementById("qtd"+index).textContent =
        quantidades[index];
    atualizarCarrinho();
}
function atualizarCarrinho(){
    const resumo =
        document.getElementById("resumo");
    let total = 0;
    let html = "";
    let temProduto = false;
    produtos.forEach((produto,index)=>{
        if(quantidades[index] > 0){
            temProduto = true;
            let subtotal =
                produto.preco * quantidades[index];
            total += subtotal;
            html += `
            <div class="linha">
                <span>
                    ${quantidades[index]}x ${produto.nome}
                </span>
                <span>
                    R$ ${subtotal.toFixed(2).replace(".",",")}
                </span>
            </div>
            `;
        }
    });
    if(!temProduto){
        html = `
        <p style="text-align:center;color:#888;">
            Nenhum lanche selecionado.
        </p>
        `;
    }
    resumo.innerHTML = html;
    document.getElementById("total").textContent =
        "R$ " + total.toFixed(2).replace(".",",");
}
function enviarPedido(event){
    event.preventDefault();
    let nome =
        document.getElementById("nome").value.trim();
    let endereco =
        document.getElementById("endereco").value.trim();
    let observacao =
        document.getElementById("observacao").value.trim();
    if(!nome){
        alert("Digite seu nome.");
        document.getElementById("nome").focus();
        return;
    }
    if(!endereco){
        alert("Digite o endereço para entrega.");
        document.getElementById("endereco").focus();
        return;
    }
    let temProduto = false;
    let total = 0;
    let mensagem =
        "🍔 *PEDIDO - ASSADINHOS DA LAURI*%0A%0A";
    mensagem +=
        "👤 *Nome:* " +
        encodeURIComponent(nome) +
        "%0A";
    mensagem +=
        "📍 *Endereço:* " +
        encodeURIComponent(endereco) +
        "%0A%0A";
    produtos.forEach((produto,index)=>{
        if(quantidades[index] > 0){
            temProduto = true;
            let subtotal =
                produto.preco * quantidades[index];
            total += subtotal;
            mensagem +=
                encodeURIComponent(
                    `${quantidades[index]}x ${produto.nome} - R$ ${subtotal.toFixed(2).replace(".",",")}`
                ) +
                "%0A";
        }
    });
    if(!temProduto){
        alert("Escolha pelo menos um lanche!");
        return;
    }
    mensagem +=
        "%0A💰 *Total: R$ " +
        total.toFixed(2).replace(".",",") +
        "*";
    if(observacao){
        mensagem +=
            "%0A%0A📝 *Observação:* " +
            encodeURIComponent(observacao);
    }
    mensagem +=
        "%0A%0A🛵 Pedido para entrega.";
    mensagem +=
        "%0A🕑 A partir das 14:00.";
    const numero =
        "5533999455745";
    const url =
        "https://wa.me/" +
        numero +
        "?text=" +
        mensagem;
    window.open(url,"_blank");
}
</script>
</body>
</html>