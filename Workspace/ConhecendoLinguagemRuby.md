Artigo[Invista em você! Saiba como a DevMedia pode ajudar sua carreira.](https://www.devmedia.com.br/conhecendo-a-linguagem-ruby/8226#modulo-mvp)

# Conhecendo a Linguagem Ruby

## Neste artigo, você irá conhecer de forma suave, a linguagem Ruby, entenda como esta linguagem de programação pode ser extremamente útil para você.

- [Artigos](https://www.devmedia.com.br/artigos/)[Canal Mais](https://www.devmedia.com.br/artigos/outros)Conhecendo a Linguagem Ruby

Ruby é uma linguagem nova em comparação às outras. Foi criada em 1995 pelo japonês Yuri Matsumoto. Uma linguagem limpa e direta toda orientada a objetos, bem simples de se aprender e trabalhar. Com muitas semelhanças ao [Perl](https://www.devmedia.com.br/perl-para-que/12787), SmallTalk e [Python](https://www.devmedia.com.br/python-por-onde-comecar/38349). **Uma Linguagem multi-plataforma**, sendo assim suportada por diversos tipos de sistemas operacionais como Linux, Windows, Solares e outros. Possui muitas features interpresantes como o Ruby Gems (Biblioteca Gratuita disponível na internet), Code Blocks( Bloco de códigos), Mixins (Reposta à herança múltipla), tipagem dinâmica e outras características. Além de ser a linguagem predileta para aprender entre os programadores Delphi.

### Ruby Gems

São bibliotecas gratuitas disponibilizadas no sourceforge.org. lá você encontra plugins para relatórios, Layouts e muito mais.

Para fazer download dos plugins diretamente pelo ruby. E só ir no WorkSpace Commander situado no 3rdRail e digitar o comando “gem install ruport” por exemplo, neste comando o 3rdRail irá buscar do site sourceforge o plugin para criação de relatórios no rails. Logo mais. Estarei mostrando melhor esta funcionalidade.

Relacionado: [Criando uma aplicação simples com Ruby On Rails](https://www.devmedia.com.br/criando-uma-aplicacao-simples-com-ruby-on-rails/34189)

### Sintaxe

A Sintaxe do Ruby é simples e exata. Sem necessidades de caracteres de término de uma instrução. Exemplo:

```
if a ==“M1”
puts “Mensagem 1”
else
puts “Mensagem 2”
end
```

### Tags

No Ruby existem duas formas de tag as que são utilizadas para estruturas de controle, loops e outras características. Eles são inseridas no HTMl. Ao compilador ler os códigos, identificará que são instruções do Rails.

```
<% Código Ruby %>
```

Exemplo :

```
<% for columEstado in Estado.content_columns %>
<%= columEstado.human_name %>
<%end%>
```

E as tags que são utilizadas para retorno de alguma informação

```
<%= Código Ruby %>
```

Exemplo:

```
<%= text_field 'usuario', 'Nome' %>
```

### Métodos

Para você criar métodos é bem simples, veja a sintaxe a baixo:

```
def meu_metodo
end
```

### Comentários

Em Ruby existem duas formas para identificar os comentários.

```
Utilizando # um comentário de uma linha.
=begin
Bloco de comentários.
=end
```

### Tipos Básicos

- Blocos de Códigos
- Números
- Booleanos
- Strings
- Constantes
- Ranges
- Array
- Símbolos
- Expressões regulares
- Procs

### Operações

Encontrei este quadro abaixo na internet. Ele exemplifica as principais operações no ruby.

### Variáveis

- Variáveis de Instância @cliente
- Variáveis Classes @@cliente
- Variáveis Globais $cliente
- Variáveis Locais Cliente

Exemplificando :

```
Locais - Opção = “Sim”
Globais - $versao = 1.5
Instância - @idade = 19
Classes - @@cont = 28
```

### Tipagem dinâmica forte

Não necessita de declarar variáveis. Sendo assim o ruby identifica o tipo dos caracteres. É considerado tipagem forte pois não aceita as misturas de tipos.

O ruby não aceita misturas como:

```
a = “a”
b = 1
c = a+b
```

Aqui estou tendo mesclar um número com um texto. Sendo assim dará um erro. Mostrando que é proibido o mesclagem.

### Code Blocks

Os Blocos de código são ao programador , de muita flexibilidade, pois pode definir como o método vai se comportar e tornou uma característica muito popular entre os programadores.

### Mixins

O Ruby suporta somente a herança simples. Mas existe o conceito de módulos que são coleções de métodos.

As classes podem conter determinados módulos assim. Herdando todos os seus métodos. Os programadores Ruby consideram essa forma a mais claro que a herança múltipla.

Exemplo:

```
class MyClass
include Enumerable
end
```

### Tratamento de campos

Para facilitar as operações Get e Set o ruby tem atalhos como:

```
Attr_reader - Set.
Attr_writer - Get.
Attr_accessor - Ambos Get e Set.
```

### Estruturas de Controle Condicionais

Aqui estarei exemplificando as estruturas condicionais, são estruturas que mudam pouco entre as linguagens, acredito que vocês se adequem rapidamente a elas.

```
IF
if i > 10
puts “maior que 10”
elseif i ==10
puts “ igual a10”
else
puts “Menor que 10”
End
Unless
unless i >= 10
puts "menor que 10"
else
puts "maior igual que 10"
end
Case
case i
when 0..5
puts “ Esta entre 0 e 5”
when 6..10
puts “ Esta entre 6 e 10”
else
puts i.to_s
end
```

### Loops

```
While
while a > 5
puts a
end
For
for a in (1..6)
puts a
end
```

Aqui demonstrarei os loops que eu utilizo mais como útil e outros.

Aqui estou encerrando, mais existem muitas outras características que possam ser mostradas. Logo estarei escrevendo mais sobre o assunto. Quem quizer mandar assuntos para que eu possa abordar aqui. Me mande uma e-mail. Um abraço para Todos. Fiquem com DEUS.

### Links Úteis

- [Plataforma de código aberto](https://sourceforge.net/) Crie, colabore e distribua.
- [Plataforma de compartilhamento e versionamento](https://github.com/).
- [Linguagem de programação Ruby Uma linguagem dinâmica](https://www.ruby-lang.org/pt/), open source com foco na simplicidade e na produtividade. Tem uma sintaxe elegante de leitura natural e fácil escrita.

### Saiba mais sobre Ruby ;)

- [Introdução ao recursos básicos da linguagem Ruby](https://www.devmedia.com.br/introducao-ao-recursos-basicos-da-linguagem-ruby/31504): Conheça os recursos básicos do Ruby e comece a criar seus primeiros blocos de código com essa linguagem
- [Tipos de dados em Ruby](https://www.devmedia.com.br/tipos-de-dados-em-ruby/33600): Neste artigo faremos uma introdução a linguagem de programação Ruby mostrando algumas das suas principais características e uma análise mais detalhada sobre os principais tipos de dados e sua sintaxe de declaração.
- [Arrays e Blocos com Ruby utilizando o IRB](https://www.devmedia.com.br/arrays-e-blocos-com-ruby-utilizando-o-irb/34268): Veja neste artigo como desenvolver em Ruby utilizando Arrays e Blocos. Os Arrays possuem diversos métodos que ajudam a facilitar o trabalho dos desenvolvedores, enquanto os blocos estão entre as grandes novidades trazidas pelo Ruby.

Tecnologias:

- Ruby

AnotarMarcar como concluído

![img](https://my.rtmark.net/img.gif?f=sync&partner=8d192082bc983b05cb53af79646518fd98e3750c921f0ae655da3dd5cb2d040f&ttl=&rurl=https%3A%2F%2Fwww.devmedia.com.br%2Fconhecendo-a-linguagem-ruby%2F8226)