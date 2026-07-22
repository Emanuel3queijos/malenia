# LGPD (Lei 13.709/2018) — Parte 1: Os Pilares (Cap. I, II e III)

## 1. Os "Personagens" da LGPD (Art. 5º)

A FGV ama trocar a função desses atores. Guarde os quatro papéis:

- **👤 Titular:** a pessoa física a quem os dados pertencem. **Pessoa jurídica NÃO é titular de dados pessoais** na LGPD (a lei protege apenas pessoa natural).
- **👑 Controlador:** quem **toma as decisões** sobre o tratamento dos dados (pode ser pessoa natural ou jurídica, de direito público ou privado). Ex.: a Dataprev.
- **🛠️ Operador:** quem **executa** o tratamento em nome do controlador, seguindo suas instruções. Ex.: uma empresa de *cloud* contratada que processa os dados da Dataprev.
- **☎️ Encarregado (DPO — Data Protection Officer):** pessoa indicada pelo controlador para ser o **canal de comunicação** entre o Controlador, os Titulares e a ANPD.

> 💡 Controlador + Operador = **"Agentes de Tratamento"** (Art. 5º, IX) — termo que a banca usa para se referir aos dois juntos.

---

## 2. A Diferença Vital dos Dados (Art. 5º, I a III)

- **📄 Dado Pessoal:** informação relacionada a pessoa natural **identificada ou identificável** (nome, CPF, IP, e-mail, placa do carro).
- **⚠️ Dado Pessoal SENSÍVEL (o prato cheio das bancas):** dado sobre **origem racial/étnica, convicção religiosa, opinião política, filiação a sindicato ou a organização de caráter religioso/filosófico/político, dado referente à saúde ou à vida sexual, dado genético ou biométrico**, quando vinculado a uma pessoa natural.
  > 💡 *Pegadinha clássica:* a FGV coloca "salário" ou "histórico de compras" como dado sensível. **NÃO É!** É dado pessoal comum. Dado sensível é o que carrega **potencial discriminatório**.
- **🔒 Dado Anonimizado:** dado que perdeu a possibilidade de associação a um indivíduo, pela utilização de meios técnicos razoáveis e disponíveis. **Não é considerado dado pessoal** para fins da LGPD — salvo se o processo de anonimização for **reversível** com os meios disponíveis.

---

## 3. Os Princípios da LGPD (Art. 6º) — onde a FGV mais pega candidato

A lei tem **10 princípios**. A banca costuma bater em três, mas vale saber os dez, porque ela adora trocar o nome de um pelo conceito de outro:

| # | Princípio | Ideia central |
|---|---|---|
| 1 | **Finalidade** | Coleta só para propósitos legítimos, específicos, explícitos e informados ao titular — nada de "coletar por coletar" |
| 2 | **Adequação** | Compatibilidade do tratamento com as finalidades informadas |
| 3 | **Necessidade (minimização)** | Coletar **apenas o mínimo estritamente necessário** para a finalidade |
| 4 | **Livre acesso** | Garantia de consulta facilitada sobre forma e duração do tratamento |
| 5 | **Qualidade dos dados** | Exatidão, clareza, relevância e atualização dos dados |
| 6 | **Transparência** | Informações claras, precisas e acessíveis sobre o tratamento |
| 7 | **Segurança** | Medidas técnicas e administrativas aptas a proteger os dados |
| 8 | **Prevenção** | Adotar medidas para **prevenir** danos, não apenas remediá-los |
| 9 | **Não discriminação** | Dados **não podem** ser usados para fins discriminatórios ilícitos ou abusivos (ex.: algoritmo de seleção que filtra candidatos por perfil biométrico) — crucial em provas de TI/IA |
| 10 | **Responsabilização e prestação de contas (*accountability*)** | O agente deve demonstrar, comprovadamente, que adotou medidas eficazes de conformidade |

---

## 4. Bases Legais — quando se pode tratar dados (Arts. 7º e 11)

**A maior pegadinha da LGPD:** *"só se pode tratar dados com consentimento"*. **MENTIRA!** O consentimento é apenas **1 das 10 hipóteses** do Art. 7º.

### Dados pessoais comuns (Art. 7º) — as 10 bases:
1. Consentimento do titular;
2. Cumprimento de obrigação legal ou regulatória pelo controlador;
3. **Pela Administração Pública**, para execução de políticas públicas previstas em lei/regulamento ou respaldadas em contratos e convênios;
4. Realização de estudos por órgão de pesquisa;
5. Execução de contrato (ou procedimentos preliminares) do qual o titular seja parte;
6. Exercício regular de direitos em processo judicial, administrativo ou arbitral;
7. Proteção da vida ou da incolumidade física do titular ou de terceiro;
8. Tutela da saúde, em procedimento realizado por profissionais/serviços de saúde;
9. **Legítimo interesse** do controlador ou de terceiro (exceto se prevalecerem direitos e liberdades fundamentais do titular);
10. Proteção do crédito.

> 🎯 **Foco de prova (Dataprev/INSS):** a Administração Pública trata a maior parte dos dados dos cidadãos **sem consentimento**, com base no cumprimento de obrigação legal/regulatória e na execução de políticas públicas (bases 2 e 3 acima) — não no consentimento do cidadão.

### Dados pessoais sensíveis (Art. 11) — regime mais restrito
Aqui as bases são bem mais limitadas: **consentimento específico e destacado**, ou, sem consentimento, apenas quando indispensável para hipóteses como cumprimento de obrigação legal, execução de políticas públicas pela Administração, estudos por órgão de pesquisa, exercício regular de direitos, proteção da vida, tutela da saúde ou **garantia de prevenção à fraude e à segurança do titular**.

> ⚠️ Repare: **"legítimo interesse" NÃO é base legal para dado sensível** — só vale para dado comum (Art. 7º, IX). Troca clássica de banca.

---

## 5. Direitos do Titular (Art. 18)

O titular pode exigir do controlador, mediante requisição facilitada e gratuita:

- Confirmação da existência de tratamento;
- Acesso aos dados;
- Correção de dados incompletos, inexatos ou desatualizados;
- **Anonimização, bloqueio ou eliminação** de dados desnecessários, excessivos ou tratados em desconformidade com a lei;
- **Portabilidade** dos dados a outro fornecedor de produto ou serviço;
- **Eliminação** dos dados pessoais tratados **com consentimento** do titular (exceto nas hipóteses de guarda obrigatória do Art. 16);
- Informação sobre as **entidades públicas e privadas** com as quais o controlador realizou uso compartilhado de dados;
- Informação sobre a **possibilidade de não fornecer consentimento** e sobre as consequências da negativa;
- **Revogação do consentimento**.

> 💡 *Atenção à nuance:* o inciso IV (anonimizar/bloquear/eliminar dados **desnecessários ou excessivos**) é diferente do inciso VI (eliminar dados tratados **com base no consentimento**). A FGV gosta de misturar os dois em uma mesma assertiva.
>
> 💡 Revogar o consentimento tem efeito **daqui para frente (ex nunc)** — **não anula** os tratamentos já realizados enquanto o consentimento era válido.

---

## 6. Bônus que costuma escapar: a ANPD

A **Autoridade Nacional de Proteção de Dados (ANPD)** é o órgão responsável por fiscalizar, orientar e sancionar o cumprimento da LGPD. Desde a Lei nº 14.460/2022, a ANPD deixou de ser um órgão vinculado à Presidência da República e passou a ser uma **autarquia de natureza especial**, com autonomia técnica, decisória, administrativa e patrimônio próprio, com sede e foro no Distrito Federal.

> 📌 Se a questão disser que a ANPD é "órgão da Presidência da República" como situação **atual**, está desatualizada — isso valia até 2022.

---

### Próximo passo
Topo mandar uma questão estilo FGV cruzando **Dado Sensível vs. Dado Comum** (com a pegadinha do "legítimo interesse") — ou já seguimos para a **Parte 2** (tratamento de dados pelo Poder Público, transferência internacional e sanções)?