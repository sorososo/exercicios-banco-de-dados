# exercicios-banco-de-dados
**Exercício nível 1 - Reconhecimento**
**Resposta:** 1 - Modelo Conceitual.
2 - Modelo Lógico.
3 - Modelo Físico.
**Exercício nível 2 - Classificação**
**Resposta:** 1 - Atributo simples.
2 - Atributo Composto.
3 - Atributo multivalorado
4 - Atributo derivado.
**Exercício nível 3 - Extração**
**Resposta:** 1 - ALUNO, PLANO e CONTRATO.
2 - data_de_inicio e situação.
3 - id_aluno, id_plano e id_contrato.
4 - CONTRATO não é somente um atributo porque possui identidade própria, possui atributos próprios e participa de regras/ciclos de vida importantes na academia.
**Exercício nível 4 - Decisão**
**Resposta:** 1 - identificador principal é id_usuario.
2 - e-mail e documento
3 - documentos como CPF, são dados sensíveis e geram riscos de privacidade se circulam como chaves. E-mail e documentos também podem mudar ou precisar de ajuste, afetando uma das principais características de um bom identificador.
4 - mesmo usando id_usuario, os atributos "e-mail" e "documento" ainda devem ter a restrição de unicidade (UNIQUE).
**Exercício nível 5 - Aplicação**
**Resposta:** 1 - entidade forte: RECEITA entidade fraca: ETAPA
2 - sequência (ou número da etapa).
3 - identificador da entidade forte (ID da RECEITA) mais a chave parcial da entidade fraca (sequência da ETAPA).
4 - RECEITA = retângulo simples ETAPA = retângulo duplo. O relacionamento entre elas deve ser um losango duplo e o atributo da chave parcial deve ter um sublinhado tracejado.
**Exercício nível 6 - Avaliação** 
**Resposta:** 1/2 - Usar o "nome" como identificador (ID) é uma fragilidade pois são homônimos e podem ter pessoas com o mesmo nome, o certo é criar um identificador substituto (tipo id_cliente). Outra fragilidade é "telefone" em uma única string pois esconde a multiplicidade de dados e deve ser transformado em atributo multivalorado. "Idade armazenada" é outra fragilidade pois a idade pode ficar desatualizada. O certo é armazenar data de nascimento e transformar idade em atributo derivado. E "endereço indivisível" é uma fragilidade pois dificulta buscas e filtros, como por rua, número etc e deve ser transformado em atributo composto.
3 - As decisões dependem do uso esperado pelo sistema. Por exemplo, se a loja só precisa de um telefone para contato rápido, um atributo simples bastaria. Se ela precisasse enviar correspondências separando por CEP da rua, o endereço composto seria obrigatório.
**Exercício desafio final** 
**Resposta:** 1 - AUTOR:nome OBRA:título USUÁRIO:nome EMPRÉSTIMO:data_retirada e data_devolução EXEMPLAR:numero_exemplar.
2 - Foram criados identificadores substitutos (chaves principais) para entidades fortes, como id_autor, id_obra, id_usuário e id_empréstimo.
3 - Existe a entidade fraca EXEMPLAR pois depende totalmente da existência da entidade forte OBRA.
4 - Os IDs (id_autor, id_obra...etc) e as datas e nomes são atributos simples. Já o relevante, é o numero_exemplar classificado como uma chave parcial.
