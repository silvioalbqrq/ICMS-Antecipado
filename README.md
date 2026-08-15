# Calculadora de ICMS Antecipado – Ceará

Ferramenta web para cálculo do **ICMS Antecipado** nas operações de entrada de mercadorias procedentes de outras unidades da federação, conforme a legislação do Estado do Ceará.

**Base legal:** Decreto nº 24.569, de 31 de julho de 1997 (RICMS/CE) – Seção XXXIV – Arts. 767 a 770.

---

## Funcionalidades

- Cálculo automático da **Base de Cálculo** (Art. 768)
- Aplicação da **alíquota interna** vigente
- Subtração do ICMS destacado na NF de origem e do ICMS do frete (quando de responsabilidade do adquirente)
- Memória de cálculo detalhada
- Aviso das principais **exceções** previstas no § 1º do Art. 767
- Interface responsiva (desktop e mobile)
- Proteção básica contra inspeção/cópia do código-fonte (mantendo a seleção e cópia do conteúdo visível)

---

## Como calcular (conforme a legislação)

### 1. Base de Cálculo (Art. 768)
```
Base = Valor da operação de entrada
     + IPI (se incidente)
     + Seguro
     + Frete
     + Outros encargos cobrados ou transferíveis ao adquirente
```

### 2. ICMS Calculado (Art. 769, I)
```
ICMS Calculado = Base × Alíquota Interna
```

### 3. ICMS a Recolher (Art. 769, II)
```
ICMS a Recolher = ICMS Calculado
                − ICMS destacado na NF de origem
                − ICMS do frete (quando de responsabilidade do adquirente)
```

> **Observação:** Caso o resultado seja negativo, o valor a recolher é considerado zero.

### Alíquota interna padrão
- **20%** (vigente no Ceará a partir de 2024 – Lei nº 18.305/2023)
- O campo é editável para permitir simulações com outras alíquotas específicas.

---

## Exceções (Art. 767, § 1º)

O pagamento antecipado **não se aplica** nas operações com mercadoria:

1. Destinada para **insumo de estabelecimento industrial**
2. Sujeita ao regime da **substituição tributária**
3. Sujeita ao **regime especial de fiscalização e controle**
4. **Sem destinatário certo**
5. **Mel de abelha**, quando destinado a estabelecimento industrial
6. Destinada a armazenamento em estabelecimento de **Operador Logístico** inscrito com CNAE 5211-7/99 e possuidor de Regime Especial de Tributação

Nas hipóteses dos itens 2, 3 e 4, aplica-se a legislação tributária específica.

---

## Recolhimento (Art. 770)

O ICMS apurado deve ser recolhido:
- Na passagem da mercadoria pelo **posto fiscal de entrada** no Estado do Ceará, ou
- No **domicílio fiscal** do contribuinte, quando este for credenciado para pagamento em domicílio.

O pagamento pode ser efetuado em qualquer instituição da rede arrecadadora credenciada, mediante **Documento de Arrecadação Estadual (DAE)** – versão rede arrecadadora ou versão eletrônica (home/office banking).

---

## Como usar

1. Abra o arquivo `icms-antecipado-ceara.html` em qualquer navegador moderno.
2. Preencha os campos da operação.
3. Clique em **Calcular ICMS Antecipado**.
4. Confira o resultado e a memória de cálculo.

Não é necessário instalar nada. O arquivo é autossuficiente (HTML + CSS + JavaScript embutidos).

---

## Arquivos do projeto

| Arquivo                        | Descrição                                      |
|--------------------------------|------------------------------------------------|
| `icms-antecipado-ceara.html`   | Calculadora completa (única página)            |
| `README.md`                    | Este arquivo de documentação                   |

---

## Avisos importantes

- Esta ferramenta é de **apoio ao cálculo**. Não substitui consultoria tributária especializada.
- Sempre confira a legislação atualizada e o enquadramento específico da operação.
- A alíquota interna modal do Ceará pode sofrer alterações. Verifique a legislação vigente na data da operação.
- O resultado do cálculo não gera documento oficial de arrecadação. Utilize os sistemas da SEFAZ-CE para emissão do DAE.

---

## Referências

- [Decreto nº 24.569/1997 – RICMS/CE](https://www.sefaz.ce.gov.br)
- Lei nº 18.305/2023 (alteração da alíquota modal para 20%)
- Portal da SEFAZ-CE: [https://www.sefaz.ce.gov.br](https://www.sefaz.ce.gov.br)

---

**Estado do Ceará** · Secretaria da Fazenda  
Ferramenta desenvolvida para fins de apoio e orientação.
