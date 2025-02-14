# APRENDENDO MARKDOWN
Respotiório contendo informações sobre o markdown para explorar esta linguagem de marcação muito utilizada atualmente em diversos projetos e principalmente no github.  
Vou deixar aqui o conhecimento obtido de dirversas fontes.

---  
## ENFATIZAR TEXTO
Como devemos enfatizar um texto no markdown

1. itálico: usamos '*' ou '_'. exemplo:
*texto em itálico*
 
_texto em itálico_

2. negrito: usamos '**' ou '__', exemplo:
**texto em negrito**

__texto em negrito__   

3. escape de caracter, exemplo de escape do asterisco usando '\':

Isso é um texto usando \*escape\*, veja como \_\_não formata\_\_ a palavra.


**RESUMO DOS ESTILOS**  
| Estilo                        | Sintaxe                | Atalho do teclado                                       | Exemplo                                      | Saída                            |
|-------------------------------|------------------------|--------------------------------------------------------|----------------------------------------------|----------------------------------|
| Negrito                       | ** ** ou __ __         | Comando+B (Mac) ou CTRL+B (Windows/Linux)              | **This is bold text**                        | Este texto está em negrito       |
| Itálico                       | * * ou _ _             | Comando+I (Mac) ou CTRL+I (Windows/Linux)              | _This text is italicized_                    | Este texto está em itálico       |
| Tachado                       | ~~ ~~                  | Nenhum                                                 | ~~This was mistaken text~~                   | Este texto contém um erro        |
| Negrito e itálico aninhado    | ** ** e _ _            | Nenhum                                                 | **This text is _extremely_ important**       | Este texto é extremamente importante |
| Todo em negrito e itálico     | *** ***                | Nenhum                                                 | ***All this text is important***             | Todo este texto é importante     |
| Subscrito                     | <sub> </sub>           | Nenhum                                                 | This is a <sub>subscript</sub> text          | Este é um texto subscrito        |
| Sobrescrito                   | <sup> </sup>           | Nenhum                                                 | This is a <sup>superscript</sup> text        | Este é um texto sobrescrito      |
| Sublinhado                    | <ins> </ins>           | Nenhum                                                 | This is an <ins>underlined</ins> text        | Este é um texto sublinhado       |

---

## DECLARAR TÍTULOS
Usamos o caracter # para representar títulos, temos títulos indo de 1 a 6.

# titulo 1;
## titulo 2;
### titulo 3;
#### titulo 4;
##### titulo 5;
###### titulo 6;

---

## CRIAR LINKS DE IMAGENS E SITES
É possível linkar coisas no markdown também, como imagens e sites, veja:

**Estrutura:**

\![titulo do link](link ou diretório)

\[link to Microsoft training](https://learn.microsoft.com/pt-br/training/paths/github-foundations/)

**EXEMPLOS:**
![github](https://img.icons8.com/?size=100&id=22989&format=png&color=000000)
  
[link to Microsoft training](https://learn.microsoft.com/pt-br/training/paths/github-foundations/)

---

## DEFINIR E CRIAR LISTAS ORDENADAS E NÃO ORDENADAS
Podemos criar listas ordenadas que começam com números ou listas não ordenadas que começam com '*' ou '-'.

**lista ordenada:**

1. First
1. Second
1. Third



**lista não ordenada e aninhada**

- First
- Second
    - nested
- Third

---

## Criar Tabelas
O markdown permite uma estruturação de tabela usando uma combinação de barras verticais e traços.

coluna 1|coluna 2
-|-
1|2
2|2

---

## Texto de citação
Para citar algo devemos usar '>'.


> Assim podemos fazer citações.

---


## HTML incorporado ao markdown
Podemos usar tags html dentro do markdown, veja uma quebra de linha por exemplo usando a tag \<br />:

estou digitando e vou quebrar a linha<br />agora mesmo.

---  

## Trabalhando com código dentro do markdown
Podemo inserir blocos de código usando '``'. veja:

Eu vou digitar um comando `git clone` e ele ficará marcado como código.

Outra opção é usar um bloco de código mesmo.

```python
def soma (*num):
    return sum(num)

print(soma(1,2,3,4,5)) # 15 

```
---  

## Notificar um desenvolvedor ou equipe usando '@'
No git podemos notificar alguém usando um @ seguido do nome de usuário para notificá-lo de algo, isso é chamado de 'menção'. Por exemplo:

Devemos proceder notificando o @devLink13 que é o codeowner desta feature antes de modificá-la sem autorização.

---  
## montiroramento de tarefas usando uma espécie de TODO interativo:
Fazemos uma lista de todo, ou de check iterativo usando a seguinte sintaxe '- [ ]' por exmeplo:

- [ ] Consetertar bugs da nova feature;
- [ ] Abrir uma issue sobre os novos temas para o mês de março;
- [ ] Fazer um pullrequest na branch main.

---  
## Comandos de barra "/"
Os comandos de barra "/" podem economizar tempo reduzindo a digitação necessária para criar um Markdown complexo.

Use comandos de barra "/" em qualquer campo de descrição ou de comentário em problemas, solicitações de pull ou discussões em que há suporte para o comando de barra "/".

comando|descrição
-|-
/code	| Insere um bloco de código Markdown. Você escolhe a linguagem.
/details	| Insere uma área de detalhes recolhível. Você escolhe o título e o conteúdo.
/saved-replies | 	Insere uma resposta salva. Você escolhe uma das respostas salvas para sua conta de usuário. Se você adicionar %cursor% à sua resposta salva, o comando de barra "/" coloca o cursor nesse local.
/table |	Insere uma tabela Markdown. Você escolhe o número de colunas e linhas.
/tasklist |	Insere uma lista de tarefas. Esse comando de barra "/" só funciona em uma descrição do problema.
/template|	Mostra todos os modelos no repositório. Você escolhe o modelo a ser inserido. Esse comando de barra funciona para modelos de problemas e para um modelo de solicitação de pull.

---  
## Alertas do markdown
O markdown possui um sistema de alertas que pode ser usado diretamente da seguinte forma:
> [!NOTE]  
> Useful information that users should know, even when skimming content.

> [!TIP]  
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]  
> Key information users need to know to achieve their goal.

> [!WARNING]  
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]  
> Advises about risks or negative outcomes of certain actions.
