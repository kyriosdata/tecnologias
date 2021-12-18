# tecnologias

Tecnologias (Engenharia de Software / UFG)

# Problema

O conjunto de tecnologias empregadas no curso de Engenharia de Software, assim como na Fábrica de Software, é constantemente atualizado e disponibilizado para os interessados. Cada tecnologia inclui nome, breve descrição, possivelmente ícone e o contexto de uso. Atualmente é empregado um documento [PDF](https://ww2.inf.ufg.br/~fabio/terreno-ferramentas.pdf) para disponibilizar tais informações, assim como um documento contendo [anotações](https://docs.google.com/document/d/1kiniQskETRJu6T3-n5gAvYfKyh11xKVsJ8FkqNSGW6g/edit#heading=h.uwtpzkmp9874). 

A estratégia atualmente empregada possui inconvenientes. O processo de atualização do documento PDF é considerado "lento", adicionalmente, dificulta a visualização em dispositivos móveis e exige habilidade “artística” para a sua produção. O cenário desejado é aquele no qual o conjunto de tecnologias é atualizado e automaticamente as mudanças são refletidas em uma página web, acessível tanto por computador de mesa quanto dispositivo móvel.

# Análise

### Problema

> facilitar a constante atualização de informações sobre as tecnologias
> empregadas com a automática produção de uma visualização
> correspondente.

### Dados

Os dados a serem atualizados estão modelados no diagrama abaixo. 

<img src="https://github.com/kyriosdata/tecnologias/blob/main/imagens/modelo.png" width="100px">

Observe que o modelo acima é suficiente para o registro tanto do conteúdo do documento 
[PDF](https://ww2.inf.ufg.br/~fabio/terreno-ferramentas.pdf)
quanto das [anotações](https://docs.google.com/document/d/1kiniQskETRJu6T3-n5gAvYfKyh11xKVsJ8FkqNSGW6g/edit#heading=h.uwtpzkmp9874).

# Design 

Uma das referências sugeridas para consulta, presente no documento de [anotações](https://docs.google.com/document/d/1kiniQskETRJu6T3-n5gAvYfKyh11xKVsJ8FkqNSGW6g/edit#heading=h.uwtpzkmp9874), é o famoso [radar](https://www.thoughtworks.com/radar)
tecnológico mantido pela ThoughtWorks. Naturalmente este radar serve de inspiração para o _design_ da página
desejada no presente trabalho. Melhor ainda, este radar permite que você construa o seu próprio a partir de 
dados fornecidos em uma planilha. Consulte [Build Your Own Radar](https://radar.thoughtworks.com/) para detalhes. 

Proposta:

> empregar ferramenta para geração automática do radar tecnológico a partir de planilhas. 

Nesta proposta, uma planilha correspondente às tecnologias a serem adotadas pelo curso e pela fábrica
são definidas em uma planilha. O portal [Build Your Own Radar](https://radar.thoughtworks.com/) é 
utilizado para manualmente fornecer a planilha atualizada e gerar o resultado correspondente. 

Uma planilha preliminar está disponível [aqui](https://docs.google.com/spreadsheets/d/1-hb4xyrwt_vGl2bVaOt7LEp2fTl3dNg2tNTJKzKf008/edit#gid=0) e
o radar correspondente [aqui](https://radar.thoughtworks.com/?sheetId=https%3A%2F%2Fdocs.google.com%2Fspreadsheets%2Fd%2F1-hb4xyrwt_vGl2bVaOt7LEp2fTl3dNg2tNTJKzKf008%2Fedit%3Fusp%3Dsharing).

Adicionalmente, a geração deste radar é realizada por código open source, disponibilizado no repositório
[build your own radar](https://github.com/thoughtworks/build-your-own-radar). Ou seja, ajustes no _design_ da página,
assim como eventuais traduções e outros elementos podem ser realizados.

