Criado para que diferentes dispositivos, que analogamente "falaria idiomas diferentes", possam se comunicar de forma.
Uma forma mais básica de tentar explicar a passagem de uma informação por um meio, relacionando ao OSI, é dizer que ela passa primeiro por todas as camadas do primeiro sistema e depois, chegando ao próximo sistema, ela passa por todas as camadas dele também, até que o encapsulamento feito no início disso possa ser desfeito depois e a informação seja assim adquirida.
## Camadas (F. E. R. T. S. A. A.)

Cada camada se comunica com outra que esteja próxima a ela. São 7 camadas no modelo OSI

1. **[[~ Camada Física do Modelo OSI]]:** Dada pelos dispositivos/meios de comunicação.
2. **Enlace:** Responsável pelo endereçamento físico do dispositivo. Aqui está incluído o MAC
3. **Rede:** Responsável pelo endereçamento lógico e estabelecimento de rotas, para que a informação possa ser transportada para o lugar correto. Aqui está o IP.
4. **Transporte:** Lida com a questão do controle do fluxo de tráfego de informações, assim como é responsável pela integridade (preservação) das informações durante esse transporte.
5. **Sessão:** Responsável por manipular a conexão entre 2 dispositivos, de forma poder iniciá-la, mantê-la ou terminá-la.
6. **Apresentação:** Faz a conversão entre diferentes tipos de códigos, envolvendo criptografia. 
7. **Aplicação:** Trata-se da interface das aplicações do computador. Está incluído nela: HTTP (http:// e https://), FTP (Transferência de arquivos) e SMTP (email).