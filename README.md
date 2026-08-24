# exercicios-banco-de-dados
**Enunciado:** Classifique cada decisão.
**Resposta:** 1 - Modelo Conceitual.
2 - Modelo Lógico.
3 - Modelo Físico.
**Enunciado:** Classifique os atributos.
**Resposta:** 1 - Atributo simples.
2 - Atributo Composto.
3 - Atributo multivalorado
4 - Atribut0 derivado.
**Enunciado:** Extraia o modelo de uma narrativa.
**Resposta:** 1 - ALUNO, PLANO e CONTRATO.
2 - data_de_inicio e situação.
3 - id_aluno, id_plano e id_contrato.
4 - CONTRATO não é somente um atributo porque possui identidade própria, possui atributos próprios e participa de regras/ciclos de vida importantes na academia.
**Enunciado:** Escolha os identificadores.
**Resposta:** 1 - identificador principal é id_usuario.
2 - e-mail e documento
3 - documentos como CPF, são dados sensíveis e geram riscos de privacidade se circulam como chaves. E-mail e documentos também podem mudar ou precisar de ajuste, afetando uma das principais características de um bom identificador.
4 - mesmo usando id_usuario, os atributos "e-mail" e "documento" ainda devem ter a restrição de unicidade (UNIQUE).
**Enunciado:** Encontre uma identidade fraca
**Resposta:** 1 - entidade forte: RECEITA entidade fraca: ETAPA
2 - sequência (ou número da etapa).
3 - identificador da entidade forte (ID da RECEITA) mais a chave parcial da entidade fraca (sequência da ETAPA).
4 - RECEITA = retângulo simples ETAPA = retângulo duplo. O relacionamento entre elas deve ser um losango duplo e o atributo da chave parcial deve ter um sublinhado tracejado.

