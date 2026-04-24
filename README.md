# una-blazor-lista12
# EcoMonitor - Projeto Blazor

## Identificação

* Nome: CAUA CORDEIRO FURST VIEIRA
* Curso: CIÊNCIA DA COMPUTAÇÃO

---

## Heurísticas de Nielsen Aplicadas

Durante o desenvolvimento do componente EcoStatus, foram aplicadas algumas heurísticas de usabilidade propostas por Jakob Nielsen:

### 1. Visibilidade do Status do Sistema

O sistema mantém o usuário informado em tempo real por meio da exibição do contador atualizado e da barra de progresso, permitindo que ele acompanhe claramente sua evolução.

### 2. Feedback Imediato do Usuário

Cada interação com o botão gera uma resposta imediata, atualizando o valor acumulado e a barra de progresso, garantindo que o usuário perceba o resultado de suas ações sem atraso.

### 3. Reconhecimento em vez de Memorização

As informações como "Pontos por ação" e "Total acumulado" são sempre exibidas na tela, evitando que o usuário precise memorizar dados.

---

## Guia de Execução

Siga os passos abaixo para executar o projeto localmente:

### 1. Abrir o terminal na pasta do projeto

### 2. Executar o comando:

bash
dotnet run


### 3. Acessar no navegador:

Copie o link exibido no terminal, normalmente:


http://localhost:xxxx


---

## Explicação Técnica

O componente EcoStatus foi desenvolvido de forma reutilizável utilizando o atributo [Parameter] do Blazor.

### Uso do [Parameter]

O [Parameter] permite que valores sejam passados de uma página para o componente, tornando-o dinâmico e reutilizável.

Exemplo:

csharp
[Parameter]
public int PesoAcao { get; set; }

[Parameter]
public string NomeAcao { get; set; }

[Parameter]
public string MensagemConquista { get; set; }


### Benefícios

* Permite criar múltiplas instâncias do componente com comportamentos diferentes
* Evita repetição de código
* Facilita manutenção e escalabilidade

### Aplicação no projeto

No arquivo principal, o componente foi reutilizado com diferentes valores:

razor
<EcoStatus NomeAcao="Reciclagem" PesoAcao="1" />
<EcoStatus NomeAcao="Plantio" PesoAcao="10" />


Cada instância mantém seu próprio estado e comportamento, demonstrando a reutilização do componente.

---

## Conclusão

O projeto demonstra conceitos fundamentais do desenvolvimento com Blazor, como:

* Componentização
* Reutilização de código
* Interatividade
* Feedback visual ao usuário

Além disso, foram aplicados princípios de usabilidade para melhorar a experiência do usuário.

---


---
