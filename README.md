# Zero Carie - Sistema de Vigilancia e Promocao da Saude Bucal Escolar

O Zero Carie e um sistema digital voltado para a vigilancia e promocao da saude bucal em ambiente escolar, com foco no monitoramento da escovacao supervisionada. A plataforma permite o registro e acompanhamento, em tempo real, da adesao das criancas a rotina de escovacao, com visibilidade por escola e por turma.

---

## Indice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Estrutura de Diretorios](#estrutura-de-diretorios)
- [Como Executar o Projeto](#como-executar-o-projeto)
  - [Pre-requisitos](#pre-requisitos)
  - [Instalacao e Execucao](#instalacao-e-execucao)
- [Autor](#autor)

---

## Sobre o Projeto

O projeto Zero Carie surgiu da necessidade de digitalizar e centralizar o controle da escovacao supervisionada nas escolas, pratica amplamente recomendada pelo Ministerio da Saude como estrategia de prevencao da carie dentaria em criancas.

Por meio do sistema, profissionais de saude e educadores conseguem:

- Registrar as escovacoes realizadas em cada turma de forma rapida e pratica.
- Acompanhar a frequencia de adesao por aluno, turma e escola.
- Visualizar relatorios e indicadores de cobertura em tempo real.
- Identificar turmas ou periodos com baixa adesao para intervencao direcionada.

O sistema busca substituir planilhas e registros fisicos por uma solucao digital acessivel, responsiva e de facil operacao por profissionais da area de saude bucal coletiva.

---

## Funcionalidades

- **Registro de Escovacoes**: Lancamento diario das escovacoes supervisionadas por turma, com data, horario e responsavel pelo registro.
- **Painel por Escola**: Visualizacao consolidada da adesao de todas as turmas de uma unidade escolar.
- **Painel por Turma**: Acompanhamento individualizado da frequencia de escovacao de cada turma ao longo do tempo.
- **Monitoramento em Tempo Real**: Os dados registrados sao refletidos imediatamente nos paineis e relatorios do sistema.
- **Indicadores de Cobertura**: Percentual de adesao calculado automaticamente com base nos registros e no numero esperado de escovacoes.
- **Controle de Acesso**: Perfis diferenciados para administradores, profissionais de saude e coordenadores de escola.
- **Historico de Registros**: Consulta ao historico completo de escovacoes por periodo, turma ou escola.

---

## Tecnologias Utilizadas

### Front-end
- **React**: Biblioteca para construcao da interface de usuario.
- **Vite**: Ferramenta de build para desenvolvimento rapido com recarga instantanea.
- **React Router DOM**: Gerenciamento de rotas e navegacao entre paginas.
- **Axios**: Cliente HTTP para comunicacao com a API do back-end.
- **CSS3**: Estilizacao responsiva e customizada da interface.

### Back-end
- **Node.js**: Ambiente de execucao do servidor.
- **Express**: Framework para construcao da API REST.
- **MongoDB**: Banco de dados NoSQL para armazenamento dos registros de escovacao, turmas e escolas.
- **Mongoose**: ODM (Object Document Mapper) para modelagem e interacao com o MongoDB.
- **CORS**: Middleware para controle de acesso entre origens distintas.

---

## Estrutura de Diretorios

```text
Projeto_Zero_Carie/
├── back-end/
│   ├── api/
│   │   ├── controllers/       # Controladores das rotas (logica de negocio)
│   │   ├── models/            # Modelos de dados (Mongoose)
│   │   ├── routes/            # Definicao das rotas da API
│   │   ├── connect.js         # Configuracao da conexao com o MongoDB
│   │   └── server.js          # Inicializacao do servidor Express
│   ├── package.json
│   └── package-lock.json
├── front-end/
│   ├── src/
│   │   ├── components/        # Componentes reutilizaveis da interface
│   │   ├── pages/             # Paginas da aplicacao (Dashboard, Escolas, Turmas, etc.)
│   │   ├── api/               # Configuracao das chamadas HTTP ao back-end
│   │   ├── App.jsx            # Gerenciamento de rotas do cliente
│   │   └── main.jsx           # Ponto de entrada da aplicacao React
│   ├── index.html
│   ├── vite.config.js
│   ├── package.json
│   └── package-lock.json
└── README.md
```

---

## Como Executar o Projeto

### Pre-requisitos

- **Node.js** versao 18 ou superior instalado na maquina.
- Conta e cluster configurado no **MongoDB Atlas** (ou instancia local do MongoDB).

---

### Instalacao e Execucao

#### 1. Clonando o repositorio

```bash
git clone https://github.com/JoaocamargooaDev/Projeto_Zero_Carie.git
cd Projeto_Zero_Carie
```

#### 2. Configurando e iniciando o Back-end

```bash
cd back-end
npm install
npm start
```

O servidor da API estara disponivel em: `http://localhost:3001`

#### 3. Configurando e iniciando o Front-end

Em um novo terminal:

```bash
cd front-end
npm install
npm run dev
```

A aplicacao web estara disponivel em: `http://localhost:5173`

---

## Autor

Desenvolvido para fins de vigilancia em saude bucal coletiva, com foco na integracao entre tecnologia e saude publica escolar.

Se este projeto foi util, sinta-se a vontade para deixar uma estrela no repositorio!
