Site para testar o algoritmo que fiz para testar um algoritmo de censura de sites em HTTP. 

[Acesse o repositório Web Proxy aqui](https://github.com/Miguel-casarin/Web-Proxy-)


### Configuração do Navegador (Firefox)
Para que o tráfego do navegador seja interceptado e processado pelas regras do proxy, é obrigatório realizar a configuração no browser. Nossos testes e validações foram executados no Mozilla Firefox seguindo as etapas abaixo:

1. Acesse as Configurações.

2. Localize Configuracoes de proxy e acesse a opção "Configurar proxy"

3. Marque a opção "Configuração manual de proxy"

4. Na caixa "Proxy HTTP", defina o endereço como localhost e defina a Porta como 5000.

5. Marque a opção "Usar este proxy também em HTTPS" (esta etapa é essencial para que o método CONNECT no connect_handler.go funcione corretamente em sites seguros).

Clique em OK para aplicar as alterações.

6. Acesse as preferências avançadas digitando "about:config" na aba de URL

7. Na aba de pesquisa de preferências procure por "network.proxy.allow_hijacking_localhost". Mude para True
