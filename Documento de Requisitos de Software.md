# 📄 Documento de Requisitos de Software

## Sistema: Hub Pessoal

---

# 1. Objetivo

O sistema tem como objetivo centralizar gestão pessoal em um único aplicativo em um tipo de gamificação, integrando:

- Finanças
- Agenda
- Entretenimento
- Informações contextuais (clima, notícias, recomendações)

O foco é organização pessoal com leve camada de personalização e recomendação.

---

# 2. Escopo

O sistema permitirá ao usuário autenticado:

- Gerenciar rendas, cartões e investimentos
- Visualizar alertas financeiros
- Criar e organizar compromissos
- Manter blocos de anotações
- Controlar consumo de filmes, séries, jogos e músicas
- Receber recomendações baseadas em datas comemorativas e gostos do usuário
- Visualizar informações externas (clima e notícias)

---

# 3. Perfis de Usuário

### 3.1 Usuário Padrão

- Pode cadastrar e gerenciar seus próprios dados.
- Não há múltiplos perfis administrativos (MVP).

---

# 4. Requisitos Funcionais

## 4.1 Autenticação

**RF-01** – O sistema deve permitir login de usuário.

**RF-02** – O sistema deve manter sessão autenticada.

## 4.2 Painel (Dashboard)

**RF-03** – O sistema deve exibir visão geral contendo:

- Recomendações de entretenimento
- Próximos compromissos
- Previsão do tempo
- Notícias
- Alertas financeiros

**RF-04** – O sistema deve gerar recomendações baseadas em datas comemorativas.

## 4.3 Módulo de Finanças

### 4.3.1 Visão Geral

**RF-05** – O sistema deve exibir:

- Fatura atual
- Saldo atual
- Projeção financeira
- Compromissos financeiros
- Simulador de gasto

### 4.3.2 Renda

**RF-06** – O usuário pode cadastrar até 10 rendas.

Cada renda deve conter:

- Nome
- Valor
- Ocorrência (semanal, mensal ou anual)

### 4.3.3 Cartões

**RF-07** – O usuário pode cadastrar até 6 cartões.

Cada cartão deve conter:

- Nome personalizado
- Banco
- Despesas (parceladas ou à vista)

### 4.3.4 Investimentos

**RF-08** – O usuário pode cadastrar até 10 investimentos.

Cada investimento deve conter:

- Nome
- Banco
- Área
- Valor investido
- Calculadora investimento (Modelos ainda à definir)

## 4.4 Módulo Agenda

### 4.4.1 Compromissos

**RF-09** – O usuário pode cadastrar até 45 compromissos.
Cada compromisso deve conter:

- Nome
- Observações
- Intervalo (diário, mensal, semestral, anual)
- Cor personalizada
- Alerta prioritário (sim/não)
- Detecção de conflito de horário

**RF-10** – O usuário pode editar compromissos.

**RF-11** – O usuário pode remover compromissos.

### 4.4.2 Bloco de Anotações

**RF-12** – O usuário pode criar até 10 blocos de anotações.

## 4.5 Módulo Entretenimento

### 4.5.1 Geral

**RF-13** – O sistema deve recomendar para o usuário filmes, séries, jogos, animes com base em:

- Em datas comemorativas
- No que ele já consumiu
- Ranking (nota)

### 4.5.2 Filmes

**RF-14** – O usuário pode:

- Marcar como assistido
    - Avaliar (nota)
    - Adicionar comentário
    - Agendar para assistir

### 4.5.3 Séries

**RF-15** – O usuário pode:

- Marcar como assistido
    - Avaliar (nota)
    - Adicionar comentário
    - Agendar para assistir

### 4.5.4 Jogos

**RF-16** – O usuário pode:

- Marcar como zerado
    - Avaliar (nota)
    - Adicionar comentário
- Definir 1 único jogo como favorito

### 4.5.5 Músicas

**RF-17** – O usuário pode cadastrar:

- Artista
- Álbum
- Nota
- Comentário

---

# 5. Requisitos Não Funcionais

**RNF-01** – O sistema deve suportar múltiplos usuários isolando dados por conta.

**RNF-02** – O tempo de carregamento do painel deve ser inferior a 2 segundos.

**RNF-03** – Dados financeiros devem ser armazenados de forma segura.

**RNF-04** – O sistema deve permitir integração com APIs externas (clima, notícias, mídia).

**RNF-05** – Interface responsiva (desktop e mobile).

---

# 

**RN-01** – Apenas 1 jogo pode ser marcado como favorito por usuário. (Apenas no **MVP**)

**RN-02** – Limites máximos de cadastro devem ser respeitados.

**RN-03** – Ao marcar filme/série para assistir, deve ser criada automaticamente uma entrada na Agenda.

**RN-04** – Alertas financeiros devem ser exibidos no painel principal.

**RN-05** –
