# Site-ESW2
Site feito em aula


# Sistema de Gestão de Estacionamento 🚗🅿️

Sistema web interativo desenvolvido para o gerenciamento de pátios de estacionamento, controle de fluxo de caixa em tempo real e visualização de indicadores gerenciais no estilo Business Intelligence (Power BI).

## 🚀 Funcionalidades

### 1. Tela de Login Segura
* Autenticação baseada em perfis de acesso (**Administrador** e **Operador de Caixa**).
* Tratamento visual de erros e opção para alternar a visualização da senha.

### 2. Mapa Interativo de Vagas (Operador de Caixa)
* Visualização gráfica em tempo real do pátio do estacionamento (vagas divididas por setores).
* **Vagas Livres (Verdes):** Ao clicar, abrem os campos de cadastro (Placa, Horário, Modelo do Veículo e Nome do Dono).
* **Vagas Ocupadas (Vermelhas):** Ao clicar, calculam automaticamente o tempo de permanência e exibem o valor atualizado da tarifa de forma dinâmica.

### 3. Painel Gerencial (Administrador)
* Dashboard analítico inspirado no Power BI, contendo:
  * Gráfico de Taxa de Ocupação Atual (Medidor).
  * Indicador de Ticket Médio Mensal.
  * Distribuição de veículos por categoria (Carros, Motos, SUVs).
  * Formas de pagamento utilizadas (PIX, Cartão, Dinheiro).
  * Gráfico misto cruzando faturamento diário com volume de veículos.
  * Caixa de **Insights Inteligentes** baseada no comportamento de lotação do pátio.

---

## 🛠️ Tecnologias Utilizadas
* **HTML5 & CSS3** (Design moderno, flexbox, grid e variáveis visuais).
* **JavaScript (Vanilla)** (Lógica de controle de estado das vagas, tempo real e validações de tela).
* **Chart.js** (Biblioteca para renderização de gráficos interativos).

---

## ⚙️ Como Executar o Projeto Localmente

1. Certifique-se de ter um navegador web moderno instalado (Chrome, Edge, Firefox).
2. Faça o download ou clone este repositório em sua máquina.
3. Certifique-se de estar conectado à internet (o projeto utiliza a CDN do Chart.js para carregar os gráficos).
4. Dê um duplo clique no arquivo **`index.html`** ou abra-o utilizando a extensão *Live Server* do VS Code.

### Credenciais de Acesso para Testes:
* **Administrador:** CPF `11111111101` | Senha: `admin`
* **Operador de Caixa:** CPF `22222222202` | Senha: `func`
