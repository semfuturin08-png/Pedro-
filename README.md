# Pedro-
Página web 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beleza Natural Premium - Produtos Orgânicos para Sua Pele</title>
    <meta name="description" content="Compre produtos de beleza natural de qualidade com frete grátis! Hidratantes, máscaras e óleos essenciais para uma rotina radiante.">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Roboto', sans-serif; line-height: 1.6; color: #333; }
        .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
        
        /* Header */
        header { background: #fff; box-shadow: 0 2px 5px rgba(0,0,0,0.1); position: fixed; width: 100%; top: 0; z-index: 1000; }
        nav { display: flex; justify-content: space-between; align-items: center; padding: 1rem 0; }
        .logo { font-size: 1.5rem; font-weight: 700; color: #007BFF; }
        .nav-links { display: flex; list-style: none; gap: 2rem; }
        .nav-links a { text-decoration: none; color: #333; font-weight: 400; }
        .cart-btn { background: #007BFF; color: white; padding: 0.5rem 1rem; border: none; border-radius: 5px; cursor: pointer; } /* Agora abre o carrinho do Shopify */
        
        /* Hero */
        .hero { background: linear-gradient(rgba(0,123,255,0.8), rgba(0,123,255,0.8)), url('https://source.unsplash.com/random/1200x600/?beauty,natural'); background-size: cover; color: white; text-align: center; padding: 150px 0 100px; margin-top: 80px; }
        .hero h1 { font-size: 3rem; margin-bottom: 1rem; }
        .hero p { font-size: 1.2rem; margin-bottom: 2rem; }
        .cta-btn { background: #FF6B35; color: white; padding: 1rem 2rem; border: none; border-radius: 5px; font-size: 1.1rem; cursor: pointer; text-decoration: none; display: inline-block; }
        
        /* Produtos */
        .products { padding: 80px 0; background: #f8f9fa; }
        .products h2 { text-align: center; font-size: 2.5rem; margin-bottom: 3rem; color: #007BFF; }
        .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .product-card { background: white; border-radius: 10px; overflow: hidden; box-shadow: 0 5px 15px rgba(0,0,0,0.1); text-align: center; padding: 1rem; }
        .product-card img { width: 100%; height: 200px; object-fit: cover; }
        .product-card h3 { margin: 1rem 0; color: #007BFF; }
        .product-card .price { font-size: 1.5rem; font-weight: 700; color: #FF6B35; margin-bottom: 1rem; }
        .product-card ul { list-style: none; text-align: left; margin-bottom: 1rem; }
        .product-card ul li { margin-bottom: 0.5rem; }
        .product-card .buy-button { min-height: 50px; margin-top: 1rem; } /* Espaço para o Buy Button */
        .testimonial { font-style: italic; margin-top: 1rem; color: #666; }
        
        /* Benefícios */
        .benefits { padding: 80px 0; text-align: center; }
        .benefits h2 { font-size: 2.5rem; margin-bottom: 3rem; color: #007BFF; }
        .benefit-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; }
        .benefit-item { padding: 2rem; }
        .benefit-item h3 { color: #007BFF; margin-bottom: 1rem; }
        
        /* Depoimentos */
        .testimonials { padding: 80px 0; background: #f8f9fa; }
        .testimonials h2 { text-align: center; font-size: 2.5rem; margin-bottom: 3rem; color: #007BFF; }
        .testimonial-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .testimonial { background: white; padding: 2rem; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); text-align: center; }
        .stars { color: #FFD700; font-size: 1.2rem; margin-bottom: 1rem; }
        .testimonial img { width: 60px; height: 60px; border-radius: 50%; margin-bottom: 1rem; }
        
        /* FAQ */
        .faq { padding: 80px 0; }
        .faq h2 { text-align: center; font-size: 2.5rem; margin-bottom: 3rem; color: #007BFF; }
        .faq-item { margin-bottom: 2rem; border-bottom: 1px solid #eee; padding-bottom: 1rem; }
        .faq-item h3 { color: #007BFF; cursor: pointer; }
        
        /* Newsletter */
        .newsletter { background: #007BFF; color: white; text-align: center; padding: 50px 0; }
        .newsletter h2 { margin-bottom: 1rem; }
        form { display: flex; justify-content: center; gap: 1rem; max-width: 500px; margin: 0 auto; flex-wrap: wrap; }
        input[type="email"] { padding: 0.8rem; border: none; border-radius: 5px; flex: 1; min-width: 200px; }
        button { background: #FF6B35; color: white; padding: 0.8rem 1.5rem; border: none; border-radius: 5px; cursor: pointer; }
        
        /* Footer */
        footer { background: #333; color: white; text-align: center; padding: 2rem 0; }
        .social-links { margin-bottom: 1rem; }
        .social-links a { color: white; margin: 0 1rem; text-decoration: none; }
        
        @media (max-width: 768px) {
            .nav-links { display: none; }
            .hero h1 { font-size: 2rem; }
            form { flex-direction: column; align-items: center; }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">Beleza Natural</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#produtos">Produtos</a></li>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
            <!-- Embed do Carrinho do Shopify aqui - Cole o código completo do Buy Button para Carrinho -->
            <div id='cart-component-SEU_ID_DO_CARRINHO'></div>
            <button class="cart-btn" onclick="document.getElementById('cart-component-SEU_ID_DO_CARRINHO').click();">Carrinho</button>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h1>Transforme Sua Rotina com Nossos Produtos Premium!</h1>
            <p>Descubra a beleza natural que sua pele merece. Orgânicos, eficazes e com 20% de desconto na primeira compra.</p>
            <a href="#produtos" class="cta-btn">Compre Agora - Desconto de 20%!</a>
        </div>
    </section>

    <section id="produtos" class="products">
        <div class="container">
            <h2>Nossos Produtos Estrela</h2>
            <div class="product-grid">
                <div class="product-card">
                    <img src="https://source.unsplash.com/random/300x200/?cream,organic" alt="Creme Hidratante Orgânico">
                    <h3>Creme Hidratante Orgânico</h3>
                    <p class="price">R$49,90</p>
                    <ul>
                        <li>Hidrata profundamente sem químicos</li>
                        <li>Indicado para todos os tipos de pele</li>
                        <li>Resultado visível em 3 dias</li>
                    </ul>
                    <p class="testimonial">"Mudou minha rotina! Pele macia o dia todo." - Ana S.</p>
                    <!-- Embed do Buy Button para este produto - Cole o código completo aqui -->
                    <div id='product-component-ID_DO_CREME' class="buy-button"></div>
                </div>
                <div class="product-card">
                    <img src="https://source.unsplash.com/random/300x200/?mask,face" alt="Máscara Facial Revitalizante">
                    <h3>Máscara Facial Revitalizante</h3>
                    <p class="price">R$29,90</p>
                    <ul>
                        <li>Renova a pele em 7 dias</li>
                        <li>Ingredientes 100% naturais</li>
                        <li>Fácil de usar em casa</li>
                    </ul>
                    <p class="testimonial">"Minha pele nunca esteve tão radiante!" - João P.</p>
                    <!-- Embed do Buy Button para este produto -->
                    <div id='product-component-ID_DA_MASCARA' class="buy-button"></div>
                </div>
                <div class="product-card">
                    <img src="https://source.unsplash.com/random/300x200/?oil,lavender" alt="Óleo Essencial de Lavanda">
                    <h3>Óleo Essencial de Lavanda</h3>
                    <p class="price">R$39,90</p>
                    <ul>
                        <li>Relaxa e equilibra a mente</li>
                        <li>Versátil para pele e aromaterapia</li>
                        <li>Puro e extraído naturalmente</li>
                    </ul>
                    <p class="testimonial">"Perfeito para noites tranquilas." - Maria L.</p>
                    <!-- Embed do Buy Button para este produto -->
                    <div id='product-component-ID_DO_OLEO' class="buy-button"></div>
                </div>
            </div>
        </div>
    </section>

    <section class="benefits">
        <div class="container">
            <h2>Por Que Escolher Nós?</h2>
            <div class="benefit-grid">
                <div class="benefit-item">
                    <h3>Entrega Rápida</h3>
                    <p>Receba em até 3 dias úteis em todo o Brasil.</p>
                </div>
                <div class="benefit-item">
                    <h3>Garantia de 30 Dias</h3>
                    <p>Satisfação garantida ou seu dinheiro de volta.</p>
                </div>
                <div class="benefit-item">
                    <h3>Pagamentos Seguros</h3>
                    <p>Cartão, boleto e Pix com criptografia SSL.</p>
                </div>
                <div class="benefit-item">
                    <h3>Frete Grátis</h3>
                    <p>Acima de R$100 em compras.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="testimonials">
        <div class="container">
            <h2>O Que Nossos Clientes Dizem</h2>
            <div class="testimonial-grid">
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <img src="https://source.unsplash.com/random/60x60/?person,woman" alt="Cliente 1">
                    <p>"Produtos incríveis! Minha pele agradece."</p>
                    <strong>- Carla M.</strong>
                </div>
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <img src="https://source.unsplash.com/random/60x60/?person,man" alt="Cliente 2">
                    <p>"Entrega rápida e qualidade top. Recomendo!"</p>
                    <strong>- Pedro R.</strong>
                </div>
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <img src="https://source.unsplash.com/random/60x60/?person,woman2" alt="Cliente 3">
                    <p>"Adorei o óleo de lavanda. Relax total!"</p>
                    <strong>- Sofia G.</strong>
                </div>
            </div>
        </div>
    </section>

    <section class="faq">
        <div class="container">
            <h2>Perguntas Frequentes</h2>
            <div class="faq-item">
                <h3>Como faço o pagamento?</h3>
                <p>Aceitamos cartão de crédito, boleto e Pix. Tudo seguro via Shopify.</p>
            </div>
            <div class="faq-item">
                <h3>Qual o prazo de entrega?</h3>
                <p>Em até 3 dias úteis para capitais, com rastreamento incluso.</p>
            </div>
            <div class="faq-item">
                <h3>Os produtos são veganos?</h3>
                <p>Sim! Todos são 100% naturais, veganos e cruelty-free.</p>
            </div>
            <div class="faq-item">
                <h3>Posso trocar ou devolver?</h3>
                <p>Claro! Garantia de 30 dias para devoluções sem custo.</p>
            </div>
        </div>
    </section>

    <section class="newsletter">
        <div class="container">
            <h2>Receba Dicas de Beleza e Ofertas Exclusivas</h2>
            <p>Inscreva-se na nossa newsletter!</p>
            <form action="https://formspree.io/f/seu-email-aqui" method="POST">
                <input type="email" name="email" placeholder="Seu email aqui" required>
                <button type="submit">Inscrever-se</button>
            </form>
        </div>
    </section>

    <footer id="contato">
        <div class="container">
            <div class="social-links">
                <a href="https://instagram.com/sua-loja">Instagram</a>
                <a href="https://facebook.com/sua-loja">Facebook</a>
                <a href="https://whatsapp.com/sua-loja">WhatsApp</a>
            </div>
            <p>Política de Privacidade | Termos de Uso | contato@belezanatural.com</p>
            <p>&copy; 2025 Beleza Natural. Todos os direitos reservados.</p>
        </div>
    </footer>

    <!-- Scripts globais do Shopify Buy Button - Cole UM script principal aqui no final do body, adaptando para todos os produtos -->
    <script type="text/javascript">
    /* Exemplo de script base - Substitua com o seu código copiado do Shopify */
    (function () {
      var scriptURL = 'https://sdks.shopifycdn.com/buy-button/latest/buy-button-storefront.min.js';
      if (window.ShopifyBuy) {
        if (window.ShopifyBuy.UI) {
          ShopifyBuyInit();
        } else {
          loadScript();
        }
      } else {
        loadScript();
      }
      function loadScript() {
        var script = document.createElement('script');
        script.async = true;
        script.src = scriptURL;
        (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(script);
        script.onload = ShopifyBuyInit;
      }
      function ShopifyBuyInit() {
        var client = ShopifyBuy.buildClient({
          domain: 'SEU_DOMINIO.myshopify.com',  // ex: belezanatural.myshopify.com
          storefrontAccessToken: 'SUA_API_KEY',  // Copie do Shopify
          appId: '6'  // Padrão para Buy Button
        });
        ShopifyBuy.UI.onReady(client).then(function (ui) {
          // Inicialize cada produto aqui, usando os IDs dos divs
          ui.createComponent('product', {
            id: [ID_DO_PRODUTO_1],  // ex: ID do Creme
            node: document.getElementById('product-component-ID_DO_CREME'),
            moneyFormat: 'R$ {{amount}}',
            options: { /* Suas customizações */ }
          });
          // Repita para os outros produtos...
        });
      }
    })();
    </script>
</body>
</html>
