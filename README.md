# Projeto Unidade II – Laboratório de Programação

- **Curso:** Ciência da Computação (UNIT)
- **Docente:** Layse Santos Souza
- **Turma:** GP0029 VNO03A
- **Avaliação:** 10/12/2026 | **Devolução:** 14/12/2026
- **Formato:** em grupo, entrega de um único arquivo `.ipynb` no Teams (Avaliação - Unidade II)

## Observações do enunciado

1. Não é permitido empréstimo de materiais, consulta a IA, conversas paralelas ou consultas durante o projeto (nota zero).
2. Deve ser feito em grupo; todos os componentes devem enviar o arquivo.
3. Arquivo fora do prazo ou que não execute será desconsiderado (nota zero).

## Questão 01 (8,0) – Sistema de atas de reuniões

Sistema para cadastrar reuniões, emitir atas e acompanhar a aprovação até a conclusão.

### Regras de negócio

- Toda reunião é documentada por uma ata.
- Cada ata tem um funcionário **emissor**.
- A ata registra: título, data de emissão, data/hora de início e término, pauta, descrição, participantes, palavras-chave, status e visibilidade.
- **2 a 10 participantes**; o emissor deve estar entre eles e deve haver ao menos mais uma pessoa.
- Participantes podem ser funcionários ou externos.
- **1 a 5 palavras-chave** por ata.
- Visibilidade: pública por padrão, podendo ser alterada para privada.
- Status: "Emitida" após a emissão; participantes podem aprovar e registrar sugestões; depois dos ajustes, passa a "Concluída".
- Permitir cadastrar, consultar e atualizar reuniões, atas, participantes, sugestões e palavras-chave.
- Interface de cadastro e menu de navegação.

### Classes (diagrama UML)

`Pessoa` (abstrata), `Funcionario`, `ParticipanteExterno`, `Reuniao`, `Ata`, `ParticipanteReuniao`, `Sugestao`, `PalavraChave`.

### Distribuição da nota

| Item | Critério | Pontos |
|------|----------|--------|
| a | Implementação das classes, atributos, métodos e relacionamentos | 3,0 |
| b | Estrutura da solução e aderência ao UML | 1,0 |
| c | Interface de cadastro e menu (menu, cadastro, consulta, atualização) | 1,0 |
| d | Funcionamento (cadastro, consulta, atualização/exibição sem erros) | 1,5 |
| e | POO (encapsulamento, herança, polimorfismo, abstração) e regras de negócio | 1,5 |
