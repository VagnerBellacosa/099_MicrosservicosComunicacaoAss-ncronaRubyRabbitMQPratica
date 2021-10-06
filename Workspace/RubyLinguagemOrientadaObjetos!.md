[
LLinguagem de Programação](https://blog.betrybe.com/linguagem-de-programacao/)

# Ruby: tudo sobre essa linguagem orientada a objetos!

- por[Cairo Noleto](https://blog.betrybe.com/author/cairo-noleto/)
- 18 de abril de 2020
- 5 minutos de leitura

A linguagem **Ruby** foi criada na década de 90 por Yukihiro “Matz” Matsumoto. Ele se inspirou nas melhores partes de outras linguagens para o seu desenvolvimento, entre elas Perl, Smalltalk, Eiffel, Ada e Lisp.

O Ruby é uma linguagem de programação orientada a objetos e foi criado para que as [pessoas que desenvolvem softwares](https://blog.betrybe.com/carreira/desenvolvedor-de-software/) entendam com facilidade como ele funciona. Não é à toa que ele ocupa a primeira posição entre as linguagens que mais crescem, com a marca de 374 novos sites, desde fevereiro de 2020, segundo as estatísticas levantadas pelo W3Techs.

Ruby pode ser utilizada para criar aplicações desktop, em sistemas embarcados e várias outras utilidades. Com o advento do desenvolvimento web na década de 2000, foi criado, em 2003, **o framework web** **Ruby on Rails, o que popularizou muito a linguagem para desenvolvimento de aplicações web**.

Para que você entenda um pouco mais sobre essa poderosa linguagem, vamos mostrar, neste conteúdo:

- [**O que é Ruby?**](https://blog.betrybe.com/linguagem-de-programacao/ruby/#1)
- [**Quais os principais conceitos dessa linguagem?**](https://blog.betrybe.com/linguagem-de-programacao/ruby/#2)
- **[Vale a pena aprender Ruby? Quais as vantagens?](https://blog.betrybe.com/linguagem-de-programacao/ruby/#3)**

Vamos lá!

O que é Ruby?

**Ruby** é uma linguagem de script, open source e multiplataforma. Portanto, pode ser utilizada em diversos ambientes, como Windows, Linus, Unix, macOS, entre outros. Ela necessita de um interpretador para ser executada. Isso significa que há um programa responsável por traduzir as instruções para a linguagem de máquina.

O Ruby é uma linguagem interpretada e orientada a objetos com tipagem dinâmica e forte. Com isso, ela é capaz de definir os tipos de uma variável ou uma função, de acordo com os valores que recebe. Além disso, conta com gerenciamento de memória automático, o que significa uma melhor otimização e performance da aplicação.

**É importante dizer que Ruby é a linguagem de programação e Ruby on Rails é um framework para o** [**desenvolvimento de aplicações web**](https://blog.betrybe.com/desenvolvimento-web/aplicacoes-web/) que utiliza a linguagem Ruby. Portanto, para aprender Ruby on Rails, é preciso conhecer como a linguagem de programação funciona.

Newsletter da Trybe

Junte-se a mais de 100.000 pessoas da nossa tribo que recebem conteúdos gratuitos e exclusivos em nossa newsletter semanal!

## Principais conceitos da linguagem Ruby?

A linguagem Ruby conta com algumas características e recursos que contribuem para torná-la fácil de aprender e trabalhar. Confira, a seguir, os principais conceitos utilizados por ela.

### Sintaxe

A sintaxe do Ruby é simples e fácil de entender. Ela também é considerada uma linguagem limpa, pois não contém vírgula ou ponto-e-vírgula para indicar o final do comando. Além disso, ao escrever uma função, por exemplo, não é necessário informar o comando return para retornar o valor. A linguagem entende que a última linha é o retorno da função.

### Ruby Gems

O Ruby Gems é uma ferramenta utilizada para o gerenciamento de pacotes que podem ser baixados gratuitamente na internet. Na prática, **é um gerenciador responsável pela distribuição e instalação de bibliotecas e módulos**, chamadas gems, desenvolvidas pela comunidade Ruby.

### Code Blocks

Code Blocks, que significa bloco de códigos, em português, é um recurso dessa linguagem que permite inserir um conjunto de instruções dentro de outra função, de forma simples e rápida. Confira um exemplo:

```ruby
# Método 

def ola_mundo & block
puts “Olá mundo!”
yield
puts “Sejam bem-vindos!”
end

# Code block que será inserido no método 

ola_mundo do
puts “Vamos aprender Ruby!”
end
﻿
```

Ao executar o código, o comando “yield” buscará o conteúdo do bloco de código olá_mundo e o executará no ponto determinado. Portanto, o retorno será:

```ruby
# Resultado do processamento

Olá mundo!
Vamos aprender Ruby!
Sejam bem-vindos!
﻿
```

### Mixins

A linguagem Ruby não trabalha com herança múltipla diretamente, ou seja, não é possível herdar de várias classes ao mesmo tempo. Esse é um recurso importante para a programação orientada a objetos. Entretanto, ela trata essa necessidade de outra maneira, por meio de um recurso chamado mixin.

Na prática, ela utiliza módulos que podem ser consumidos em uma classe e, dessa forma, permitir a herança múltipla. Confira o exemplo, a seguir.

```ruby
# Primeiro módulo

module Primeiro
  def metodoA
  end
end

# Segundo módulo

module Segundo
  def metodoB
  end
end

# Classe que permite incluir vários módulos

class MesclarModulos
  include Primeiro
  include Segundo
    def metodoC
    end
end

# Consumo da classe MesclarModulos
  
  resultado = MesclarModulos.new
  resultado.metodoA
  resultado.metodoB
  resultado.metodoC
```

Vale a pena aprender Ruby? Quais as vantagens?

Conforme as estatísticas levantadas pelo [site W3Techs](https://w3techs.com/), **o Ruby ocupa a quarta posição entre as linguagens mais utilizadas para o desenvolvimento de aplicações back-end no mundo**. Entretanto, existem outras áreas que utilizam essa linguagem, como para desenvolver simuladores, modelagem 3D, entre outras. Confira, a seguir, as principais razões pelas quais vale a pena aprender essa [linguagem orientada a objetos](https://blog.betrybe.com/tecnologia/poo-programacao-orientada-a-objetos/).

### Facilidade de aprendizado

A linguagem Ruby é fácil de aprender, **pois sua sintaxe é bem limpa e intuitiva**. Além disso, é a base para a utilização de outros frameworks para o desenvolvimento de aplicações web, como o Ruby on Rails.

### Manutenção do código descomplicada

Outra vantagem dessa linguagem é a facilidade para fazer a manutenção do código. Isso é possível em razão de a sua sintaxe ser simples e compreendida facilmente por qualquer pessoa que desenvolva softwares. Dessa forma, **evita-se a necessidade de reescrever códigos por falta de compreensão da lógica de programação** utilizada por outra pessoa.  

### Ampla possibilidade de utilização

**Existem diferentes** [**tipos de aplicações que podem ser desenvolvidas com essa linguagem**](https://www.ruby-lang.org/pt/documentation/success-stories/). Por isso, grandes empresas fazem uso dessa tecnologia. Um exemplo é o Google, com o programa Google SketchUp, que utiliza a linguagem em diversas funcionalidades em sua macro API de script. Outra empresa que utiliza a linguagem é a Siemens, em um projeto sobre robótica.

Além disso, as [empresas brasileiras](https://github.com/lucascaton/empresas-brasileiras-usando-ruby) também fazem parte do grupo que utiliza essa linguagem em seu ambiente de desenvolvimento, entre elas estão: Locaweb, Resultados Digitais, Rock Content, RunRun.it, Stefanini e muitas outras.

### Oferece performance e segurança

As características da linguagem, como **produzir um código limpo, oferecer recursos de alocação de memória**, entre outras, contribuem para aumentar a performance e a segurança da aplicação. Além disso, há outras funções que ajudam nesse desempenho, como a capacidade de carregar bibliotecas dinamicamente, conforme a disponibilidade do recurso necessário no sistema operacional.

### Utilizar o framework Ruby on Rails

Como mencionamos, Ruby é a linguagem de programação utilizada no Ruby on Rails. Portanto, para [desenvolver aplicações web](https://blog.betrybe.com/carreira/programacao-para-iniciantes/) com essa tecnologia, é preciso saber como ela funciona. De acordo com as estatísticas apresentadas no site Built With, **existem mais de 2,4 mil sites no mundo que utilizam o Rails**.

Vale ressaltar que existem outros frameworks no mercado que também utilizam a linguagem Ruby. São utilizados para aplicações web, como o Sinatra, o Padrino, Grape, entre outros.

### Comunidade ativa

A linguagem Ruby é open source e **conta com uma grande comunidade na área de desenvolvimento.** Portanto, existem que podem ajudar com as dúvidas sobre o uso da tecnologia. Ou seja, estão empenhadas em apresentar melhorias e atualizações para o aprimoramento da linguagem.

O Ruby é uma linguagem de programação que oferece diversas características que permitem a criação de aplicações poderosas para diferentes finalidades, entre elas, a de criar aplicações web com o framework **Ruby on Rails** ou outro semelhante.

Já que você se interessou por este conteúdo sobre linguagem de programação, confira [o que é um framework, como ele funciona e quais suas vantagens](https://blog.betrybe.com/framework-de-programacao/o-que-e-framework/)!

[Share](https://www.facebook.com/sharer.php?u=https://blog.betrybe.com/linguagem-de-programacao/ruby/)

[Tweet](https://twitter.com/share?&text=Ruby%3A tudo sobre essa linguagem orientada a objetos!&via=betrybe&url=https://blog.betrybe.com/linguagem-de-programacao/ruby/)

[Share](mailto:?subject=Ruby%3A tudo sobre essa linguagem orientada a objetos!&body=Ruby%3A tudo sobre essa linguagem orientada a objetos! https://blog.betrybe.com/linguagem-de-programacao/ruby/)

[Share](https://www.linkedin.com/shareArticle?mini=true&url=https://blog.betrybe.com/linguagem-de-programacao/ruby/)

[Share](https://t.me/share/url?&text=Ruby%3A tudo sobre essa linguagem orientada a objetos!&url=https://blog.betrybe.com/linguagem-de-programacao/ruby/)