# Aula 2 - Introdução à Segurança da Informação

## ISO

### Definição
ISO (International Organization for Standardization) é uma organização internacional que define normas para garantir a qualidade, segurança e eficiência de produtos, serviços e sistemas.

### ISO 27001 - *Information Security Management System* (ISMS)

Especifica os **requisitos para estabelecer, implementar, manter e melhorar** continuamente um sistema de gestão de segurança da informação (SGSI).

Nota: Pode ser utilizado para análise e/ou **certificação**.

### ISO 27002

Especifica **um código de boas práticas para a gestão da segurança da informação**, possui:

- Um conjunto de controlos de segurança;
- As melhores práticas de segurança atuais;

Nota: **Não pode ser utilizado** para análise e/ou certificação.

### ISO 9001 - *Quality Management System* (QMS)

Especifica os requisitos para um sistema de gestão da qualidade, onde uma organização precisa demonstrar a sua capacidade para fornecer produtos que atendam aos requisitos do cliente e regulamentares aplicáveis.

Contém os seguintes **princípios**:
 - PDCA (*Plan*, *Do*, *Check*, *Act*);
 - Abordagem por processos;
 - Pensamento baseado em riscos;

## Sistema de Gestão

É uma ferramenta que permite a uma organização **controlar e melhorar o seu desempenho**, através de uma avaliação da eficácia dos processos.

Para implementar um sistema de gestão, é **necessário**:
- **Planear**:
  - Compreender a organização e o seu contexto;
  - Compreender as necessidades e expectativas das partes interessadas;
  - Determinar o âmbito do sistema de gestão;
  - Estabelecer a liderança política do sistema de gestão;
  - Suporte de recursos, competência, consciencialização, comunicação e informação documentada;
- **Fazer**:
  - Planeamento e controlo operacional;
  - Avaliação dos riscos da segurança da informação;
  - Tratamento dos riscos;
- **Verificar**:
  - Monitorização, medição, análise e avaliação;
  - Auditoria interna;
  - Revisão pela gestão;
- **Agir**:
  - Melhoria contínua;
  - Revisão pela gestão.

## Sistema de Gestão integrado

É um sistema que permite a uma organização **integrar vários sistemas de gestão** (qualidade, ambiente, segurança, etc.) uniformizando os procedimentos.


## Annex A

Pode ser usado como uma *checklist* dos controlos do ISO 27001.

## Controlos de Segurança

A seleção dos controlos a aplicar **depende de**:
 - Fatores de negócio;
 - Processos de negócio;
 - Âmbito do ISMS (ex: pessoas, processos, tecnologia);

# Gestão de Continuidade de Negócio

É a capacidade de uma organização **continuar a operar** após um incidente, garantindo a **recuperação** das operações críticas.

## Business Continuity Management (BCM) - ISO 22301

É um processo que identifica **ameaças potenciais** para uma organização e os **impactos** que essas ameaças podem ter sobre as operações da organização.

### Lifecycle

Pode ser dividido em várias fases:
- **Análise de risco e impacto**;
- **Desenvolvimento de estratégias**;
- **Implementação de planos**;
- **Teste e Validação**;
- **Manutenção e revisão**.

# A avaliação e gestão de riscos

## Gestão de riscos

Gestão de riscos tem como objetivo permitir à organização **atingir os objetivos** a que se propôs, mantendo em segurança os sistemas de informação que guardam, processa ou transmitem informação.

Nota: É um processo, **não um projeto**, ou seja, é contínuo.

## Avaliação de riscos

A avaliação de riscos é um **projeto** que tem como objetivo identificar, analisar e avaliar os riscos (custos, benefícios, impactos, etc.) associados a um sistema.

Pode ser feita a:
- Processos e sistemas implementados;
- Novos sistemas a implementar;

É preciso:
 - Identificar ameaças;
 - Identificar vulnerabilidades;
 - Identificar o impacto;

Tem como resultado:
 - Identificação das **ameaças** e **valorização dos riscos**;
 - Identificação de **formas de mitigar** os riscos;
 - Análise **custo-benefício** das mitigações.

Em termos de **custos**:
- Custo para correção de problemas de um sistema é **proporcionalmente direto** á fase de desenvolvimento em que o problema é detetado;
- Custos **inerentes às consequências para o negócio** (ex: confiança, disponibilidade, etc.);

Para quantificar o risco pode ser de forma:
- **Qualitativa** (níveis de valores);
- **Quantitativa** (valor numérico);

A probabilidade pode ser estimada, através de:
 - Dados e *input* interno;
 - Dados externos;

### Valorização dos ativos

Atribuição de um **nível de importância** a um ativo (um bem que a empresa possui), de forma a perceber o impacto que a sua perda pode ter na organização.

| Nível | Descrição                                                                               |
| ----- | --------------------------------------------------------------------------------------- |
| 1     | Baixo: O processo executará normalmente, podendo existir pequenos impactos na operação. |
| 2     | Médio: O processo executará com dificuldades, podendo existir impactos na operação.     |
| 3     | Alto: O processo não executará, existindo impactos graves na operação.                  |
| 4     | Muito Alto: O processo não executará, comprometendo acordos comerciais.                 |

### Tipos de riscos

Existem dois tipos de riscos:
- **Risco Operacional**: é o risco de perda resultante de processos internos, pessoas e sistemas. O seu valor é calculado da seguinte forma `Risco(O) = Probabilidade * Impacto Operacional`;
- **Risco Financeiro**: é o risco de perda resultante de flutuações de mercado, taxas de juro, taxas de câmbio, etc. O seu valor é calculado da seguinte forma `Risco(F) = Probabilidade * Impacto Financeiro`;

(Parou no Slide 72)

### Avaliação de Riscos - Exercício de Grupo

1. Escolher uma área/sistema da Universidade
2. Identificar possíveis
   - Ameaças
   - Vulnerabilidades
   - Riscos
3. Identificar controlos a implementar

#### Exemplo do Sistema autenticação
- **Ameaças**:
  - Inundações no data center;
  - *Hacking*
- **Vulnerabilidades**:
  -  Disponibilidade e Integridade;
  -  C.I.A. (Confidencialidade, Integridade, Disponibilidade);
- **Riscos**:
  - Sem redundância de dados e sem *backups*; 
  - SQL Injection;
- **Identificação de controlos a implementar**:
  - Considerar a mudança de localização do data center ou implementar um sistema de deteção de inundações; 
  - Sistema de deteção de intrusões (IDS);
  - Implementação de um sistema de login robusto;

#### Exemplo do Paco
- **Ameaças**:
  - Engenharia Social;
  - Corrupção de dados p/ *hackers*;
  - Roubo de informação p/ *hacking*;
- **Vulnerabilidades**:
  - Falta de formação aos funcionários para detetar ataques por engenharia social e phishing; 
  - Falta de controlo de acessos;
- **Riscos**:
  - Informação pessoal de alunos e docentes comprometida;
  - Serviço inoperacional por longos períodos de tempo;
  - Comprometimento de outros serviços que utilizem as mesmas credenciais em caso de roubo de informação;
- **Identificação de controlos a implementar**:
  - Formação dos funcionários para detetar ataques por engenharia social e phishing;
  - Políticas de controlo de acessos robustas;
  - Sistemas de redundância de dados;
  - Sistemas de *backups* e verificação de integridade;