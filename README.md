# AV1 - Reescrita (Entrega do Grupo)

**Descrição**
Projeto reescrito do zero como entrega da Avaliação 1 (AV1). Esta implementação fornece uma ferramenta de linha de comando para gerenciar registros de alunos (carregar CSV), calcular médias, identificar o melhor aluno e exportar relatórios em CSV/JSON.

**Motivação**
Reescrita original e independente, preservando funcionalidade comum esperada para trabalhos acadêmicos de introdução à programação: leitura de arquivo, manipulação de dados, geração de relatório e testes automatizados.

**Conteúdo**
- `src/` - código-fonte Python
- `tests/` - testes unitários (pytest)
- `sample_data/` - exemplo de CSV com alunos
- `README.md` - este arquivo
- `CONTRIBUTORS.md` - lista de autores e matrículas
- `CHANGELOG.md` - histórico de alterações
- `AV1-reescrita.zip` - pacote preparado para envio (gerado)

## Como executar

Recomendado: criar um ambiente virtual Python 3.8+:

```bash
python -m venv .venv
source .venv/bin/activate  # ou .venv\Scripts\activate no Windows
pip install -r requirements.txt
```

Executar a aplicação (exemplo):
```bash
python -m src.main --input sample_data/students.csv --report out/report.csv --format csv
```

Opções principais:
- `--input` : caminho do CSV de entrada (obrigatório)
- `--report` : caminho do arquivo de saída (opcional)
- `--format` : `csv` ou `json` (padrão: csv)
- `--top` : imprime o melhor aluno

## Exemplos
Gerar relatório CSV:
```bash
python -m src.main --input sample_data/students.csv --report out/report.csv --format csv
```

Mostrar melhor aluno:
```bash
python -m src.main --input sample_data/students.csv --top
```

## Testes
Para rodar os testes:
```bash
pip install -r requirements.txt
pytest -q
```

## Observações
Este código foi escrito como entrega original do grupo e pode/ deve ser adaptado para o escopo específico pedido pelo professor. Se quiser que eu adapte a lógica (ex.: regras de cálculo de média, notas por componente, interface gráfica), posso modificar diretamente.
