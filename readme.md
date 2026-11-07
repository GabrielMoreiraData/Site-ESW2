
---

### **1. Requisitos Funcionais (RF)**

*O que o sistema faz (as funcionalidades entregues ao usuário).*

* **RF01 - Autenticação por Perfil:** O sistema deve permitir o acesso de diferentes tipos de usuários através de CPF e senha, redirecionando automaticamente para o painel correspondente (Administrador ou Operador de Caixa).
* **RF02 - Credenciais de Acesso Predefinidas:** O sistema deve validar o acesso do Administrador (`11111111101` / `admin`) e do Operador (`22222222202` / `func`).
* **RF03 - Mapa Interativo do Pátio:** O operador deve visualizar um mapa gráfico contendo as vagas do estacionamento, divididas visualmente por estados (livres ou ocupadas).
* **RF04 - Cadastro de Entrada de Veículos:** Ao clicar em uma vaga livre, o operador deve poder registrar a entrada preenchendo placa, horário, modelo do veículo e o nome do dono.
* **RF05 - Atualização Dinâmica de Ocupação:** O sistema deve atualizar em tempo real o status da vaga selecionada para ocupada (cor vermelha) e incrementar os contadores de lotação do pátio.
* **RF06 - Cálculo Dinâmico de Tarifas (Simulador de Permanência):** O sistema deve calcular o valor a pagar com base no tempo de permanência do veículo, aplicando aumentos tarifários periódicos de forma simulada.
* **RF07 - Checkout e Liberação de Vaga:** Ao clicar em uma vaga ocupada, o sistema deve exibir o extrato/ticket de cobrança com os dados do veículo e o valor total acumulado, permitindo registrar o pagamento e liberar a vaga novamente para o estado livre (cor verde).
* **RF08 - Dashboard Gerencial Estilo BI (Administrador):** O painel do administrador deve exibir indicadores visuais avançados, incluindo gráficos de taxa de ocupação (medidor/gauge), distribuição de veículos por categoria, formas de pagamento, desempenho financeiro semanal e uma seção de insights inteligentes.

---

### **2. Requisitos Não Funcionais (RNF)**

*Como o sistema se comporta (qualidade, desempenho, restrições e tecnologias).*

* **RNF01 - Arquitetura Single Page Application (SPA):** Toda a aplicação deve rodar em um único arquivo estruturado (`index.html`), realizando a transição de telas e gerenciamento de estados de forma fluida via manipulação do DOM por JavaScript, sem recarregamento de página.
* **RNF02 - Pilha Tecnológica Client-Side:** O sistema deve ser construído utilizando tecnologias web padrão: **HTML5** para estrutura, **CSS3** para estilização moderna (com gradientes, sombras e layouts em Grid/Flexbox) e **JavaScript (Vanilla)** para a lógica de negócio e controle de tempo real.
* **RNF03 - Dependência de Bibliotecas Externas:** A renderização dos gráficos analíticos do painel administrativo depende da biblioteca externa **Chart.js** (carregada via CDN), exigindo conexão ativa com a internet para sua correta exibição.
* **RNF04 - Usabilidade e Design Responsivo:** A interface deve seguir um padrão visual moderno, limpo e intuitivo (inspirado em layouts profissionais de login e painéis corporativos de Business Intelligence), proporcionando feedback visual imediato ao interagir com os elementos (hover, estados de erro em campos e cores indicativas de status).
* **RNF05 - Portabilidade e Compatibilidade:** O sistema deve ser executado diretamente em qualquer navegador web moderno (Chrome, Edge, Firefox, etc.) sem a necessidade de instalação prévia de servidores de aplicação ou motores de banco de dados locais para testes básicos.
