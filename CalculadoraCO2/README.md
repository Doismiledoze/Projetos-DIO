# 🌿 Calculadora de Emissão de CO₂

Uma aplicação web interativa que calcula as emissões de CO₂ geradas em viagens terrestres, ajudando você a tomar decisões mais sustentáveis e a compreender o impacto ambiental de seus deslocamentos.

## 📝 Licença

> **⚠️ AVISO**: Este projeto é uma adaptação do repositório original em:
>
> **[github.com/PabloNunes/CalculadoraCO2](https://github.com/PabloNunes/CalculadoraCO2)**
>
> **Autor Original**: [Pablo Nunes](https://github.com/PabloNunes)
>
> Todos os direitos autorais e créditos pelo conceito, lógica e implementação original pertencem ao repositório mencionado acima.

Se você está usando este código, é importante reconhecer a autoria original e linkar para o repositório principal.

## 📋 Sobre o Projeto

A **Calculadora de Emissão de CO₂** é uma ferramenta educativa que permite aos usuários:

- **Calcular emissões**: Determine a quantidade de CO₂ emitida em uma viagem entre duas cidades brasileiras
- **Comparar modalidades**: Veja como diferentes meios de transporte (bicicleta, carro, ônibus e caminhão) impactam o meio ambiente
- **Avaliar economia**: Conheça quanto de CO₂ você economiza ao escolher alternativas mais sustentáveis
- **Compensação**: Calcule a quantidade de créditos de carbono necessários para compensar as emissões
- **Geolocalização automática**: A distância é preenchida automaticamente para rotas conhecidas entre cidades brasileiras

## 🎯 Funcionalidades

### 1. **Cálculo de Distância**

- Banco de dados com rotas entre cidades brasileiras
- Busca automática de distâncias ao selecionar origem e destino
- Opção de inserir distância manualmente para rotas não cadastradas

### 2. **Múltiplas Modalidades de Transporte**

- 🚲 **Bicicleta**: 0 kg CO₂/km (zero emissão)
- 🚗 **Carro**: 0,12 kg CO₂/km
- 🚌 **Ônibus**: 0,089 kg CO₂/km
- 🚚 **Caminhão**: 0,96 kg CO₂/km

### 3. **Análise Comparativa**

- Comparação de emissões entre todos os meios de transporte
- Visualização percentual em relação ao carro (baseline)
- Ranking de eficiência ecológica

### 4. **Créditos de Carbono**

- Cálculo automático de créditos necessários para compensação
- Estimativa de preço em Reais (R$) para neutralização
- Base: 1 crédito = 1.000 kg de CO₂

## 🛠️ Estrutura Técnica

```[text]
CalculadoraCO2/
 ├── index.html # Estrutura HTML principal
 ├── css/
 │ └── style.css # Estilos com paleta eco-friendly
 ├── js/
 │ ├── app.js # Lógica principal da aplicação
 │ ├── config.js # Configurações e constantes
 │ ├── calculator.js # Funções de cálculo de emissões
 │ ├── ui.js # Manipulação do DOM e interface
 │ └── routes-data.js # Base de dados de rotas brasileiras
 └── .github/ # Configurações do repositório
 ```

### Componentes Principais

#### **config.js**

Define fatores de emissão por modo de transporte, metadados visuais e configurações de créditos de carbono.

#### **calculator.js**

Contém todas as lógicas de cálculo:

- Emissão de CO₂ por modalidade
- Comparação entre modos de transporte
- Cálculo de economia e créditos de carbono
- Estimativa de preços

#### **ui.js**

Gerencia a interface do usuário:

- Formatação de números e moeda brasileira
- Renderização de resultados
- Animações e transições
- Controles de visibilidade de elementos

#### **app.js**

Inicializa a aplicação:

- Popula a lista de cidades
- Configura auto-preenchimento de distância
- Gerencia submissão de formulários
- Orquestra as operações de cálculo

#### **routes-data.js**

Base de dados contendo:

- Rotas entre capitais brasileiras
- Rotas regionais em estados como São Paulo
- Distâncias em quilômetros

## 🚀 Como Usar

1. **Selecionar Origem**: Digite ou selecione a cidade de origem na lista de sugestões
2. **Selecionar Destino**: Escolha a cidade de destino
3. **Distância**: A distância será preenchida automaticamente ou insira manualmente
4. **Modal de Transporte**: Escolha o meio de transporte (bicicleta, carro, ônibus ou caminhão)
5. **Calcular**: Clique no botão de envio para obter os resultados

## 📊 Resultados Apresentados

Após o cálculo, você visualizará:

- **Rota**: Origem e destino selecionados
- **Distância**: Quilometragem da viagem
- **Emissão Total**: Quantidade de CO₂ emitida em kg
- **Economia**: (Se aplicável) Quanto de CO₂ você economiza vs. carro
- **Comparação**: Emissões de todas as modalidades para a mesma rota
- **Créditos de Carbono**: Quantidade necessária para compensação
- **Preço da Compensação**: Estimativa em Reais

## 🎨 Design

A aplicação utiliza uma paleta de cores eco-friendly:

- **Verde primário**: #10b981 (sustentabilidade)
- **Verde secundário**: #059669 (contraste)
- **Verde accent**: #34d399 (destaques)
- **Gradiente de fundo**: Verde ao amarelo (natureza)

A interface é **responsiva** e otimizada para dispositivos móveis e desktop.

## 💡 Fatores de Emissão

Os fatores de emissão utilizados são baseados em estudos científicos sobre transporte:

| Modalidade | Emissão | Observação |
|-----------|---------|-----------|
| Bicicleta | 0 kg/km | Zero emissão carbônica |
| Ônibus | 0,089 kg/km | Transporte coletivo eficiente |
| Carro | 0,12 kg/km | Referência de comparação |
| Caminhão | 0,96 kg/km | Maior emissão por km |

## 🌱 Sustentabilidade

Cada km percorrido tem um custo ambiental. Esta ferramenta foi desenvolvida para:

- ✅ Aumentar consciência sobre emissões de carbono
- ✅ Incentivar escolhas mais sustentáveis
- ✅ Calcular compensações necessárias
- ✅ Promover educação ambiental

## 🔧 Desenvolvimento

Este é um projeto de front-end puro, sem dependências externas. Funciona com:

- HTML5
- CSS3 com variáveis customizadas
- JavaScript vanilla (ES6+)

Não requer build tools ou servidores de backend para operação básica.
