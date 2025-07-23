## Erros da progamação

Este repositórioo fornece uma visão geral dos erros mais comuns ao programar. Aqui, você encontrará explicações, exemplos de código e soluções para erros de sintaxe, TypeError, e outros problemas frequentes.

(Utilizei a linguagem python para criar os erros como exmeplo, porém outras linguagens podem possuir outros erros!!!)


## SyntaxError
**Descrição**: Ocorre quando o código viola as regras de sintaxe do Python, como parênteses ou aspas faltando e palavras escritas erradas.

**Exemplo**:
```python
print("Olá, mundo"  # Parêntese faltando
```
**Erro**: `SyntaxError: unexpected EOF while parsing`

**Solução**: Verifique se todos os parênteses, colchetes e chaves estão fechados corretamente. Além de verificar palavras escritas e outros.

**Código Corrigido**:
```python
print("Olá, mundo")
```


## TypeError
**Descrição erro**: Acontece quando uma operação é realizada com tipos de dados diferentes.

**Exemplo**:
```python
numero = 5
texto = "10"
resultado = numero + texto
```
**Erro**: `TypeError: unsupported operand type(s) for +: 'int' and 'str'`

**Solução**: Converta os tipos de dados para serem compatíveis antes da operação.

**Código Corrigido**:
```python
numero = 5
texto = "10"
resultado = numero + int(texto)  # Converte texto para inteiro
print(resultado)  # Saída: 15
```

## NameError
**Descrição erro**: Ocorre quando uma variável ou função é usada antes de ser definida.

**Exemplo**:
```python
print(nome)  # Variável 'nome' não foi definida
```
**Erro**: `NameError: name 'nome' is not defined`

**Solução**: Certifique-se de que a variável ou função foi definida antes de usá-la.

**Código Corrigido**:
```python
nome = "Python"
print(nome)  # Saída: Python
```

## IndentationError
**Descrição erro**: Ocorre quando a indentação do código está incorreta, já que Python usa indentação para definir blocos de código.

**Exemplo**:
```python
def calcular():
print("Erro de indentação")  # Sem indentação
```
**Erro**: `IndentationError: expected an indented block`

**Solução**: Use 4 espaços (padrão PEP 8) para indentar blocos de código.

**Código Corrigido**:
```python
def calcular():
    print("Agora está correto")  # Indentado com 4 espaços
```

## ModuleNotFoundError
**Descrição erro**: Ocorre quando um módulo ou biblioteca não é encontrado, geralmente devido a instalação ausente ou importação incorreta.

**Exemplo**:
```python
import pandas
```
**Erro**: `ModuleNotFoundError: No module named 'pandas'`

**Solução**: Instale o módulo necessário usando pip e verifique se o ambiente virtual está ativo.

**Comando para Instalação**:
```bash
pip install pandas
```

**Código Corrigido**:
```python
import pandas as pd
df = pd.DataFrame({'coluna': [1, 2, 3]})
print(df)
```

## Contribuições
Sinta-se à vontade para contribuir com mais exemplos de erros ou soluções! Para começar:
1. Faça um fork deste repositório.
2. Adicione novos exemplos ou correções no `README.md`.
3. Envie um pull request.

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).