# Base de dados do portal Inteligência UFF

Este repositório contém **apenas os dados publicados** do portal
[Inteligência UFF](https://inteligencia.fanara.com.br) — o índice de atos
normativos extraído dos Boletins de Serviço da Universidade Federal
Fluminense.

> ⚠️ **Gerado automaticamente. Não edite estes arquivos à mão.**
> Qualquer alteração manual é sobrescrita na próxima publicação.

## Arquivos

| Arquivo | O que é |
|---|---|
| `portal-data.json` | O índice completo de atos, no formato que o portal consome. |
| `atos.csv` | Os mesmos atos em planilha, para quem quiser abrir no Excel ou no LibreOffice. |

## Para que este repositório existe

O portal tem duas peças que precisam ler esse índice de um endereço público,
sem senha:

1. **O importador do servidor**, que roda por agendamento duas vezes por dia e
   carrega os atos novos no banco.
2. **O modo de contingência do site**, que roda no navegador do visitante
   quando o banco de dados está fora do ar.

O código-fonte do portal fica em outro repositório, que pode estar fechado.
Separar os dados do código permite que essas duas peças continuem funcionando
sem expor o código e sem precisar de chave de acesso.

## De onde vêm os dados

São extraídos dos **Boletins de Serviço da UFF**, publicados oficialmente em
<https://boletimdeservico.uff.br>. Este repositório não é uma fonte oficial da
Universidade: é um índice derivado, mantido de forma independente, e a fonte
de verdade é sempre o boletim original em PDF — cada ato no arquivo traz o
link para o seu.

## Atualização

Publicado automaticamente todo dia, por volta das 19h10 (horário de Brasília),
quando há boletim novo. Se não houve mudança, nada é publicado e a data do
último commit fica parada — isso é normal.
