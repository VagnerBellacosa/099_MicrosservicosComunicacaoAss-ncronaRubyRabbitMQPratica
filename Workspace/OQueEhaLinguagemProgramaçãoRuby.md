# O que é a Linguagem de Programação Ruby?

Veja neste artigo o que é a linguagem de programação Ruby.

 cerca de 1 ano atrás

[Artigos](https://www.treinaweb.com.br/blog)O que é a Linguagem de Programação Ruby?

Criada no Japão em 1995 por Yukihiro “Matz” Matsumoto, a linguagem de Programação Ruby é uma linguagem dinâmica, open source, inspirada em linguagens como [Python](https://www.treinaweb.com.br/blog/o-que-e-python/), Perl, Lisp, entre outras, com foco na simplicidade e na produtividade.

Muito similar em vários aspectos com o Python, possui uma sintaxe elegante, de leitura natural e de fácil escrita, assim como diz em seu site.

Multiplataforma, o Ruby possui uma excelente curva de aprendizagem.



![Ruby on Rails Básico](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/ruby-on-rails.svg)

##### CursoRuby on Rails Básico

[Conhecer o curso](https://www.treinaweb.com.br/curso/ruby-on-rails-basico)

## Características da Linguagem de Programação Ruby

Conforme dito em seu site, foi em 2006 que o Ruby atingiu uma aceitação massiva, com a formação de grupos de usuários em todas as principais cidades do mundo e com as conferências sobre Ruby com lotação esgotada. Desta forma, o Ruby ganhou muita força nos últimos anos, tornando uma linguagem amplamente utilizada por muitos programadores que desejam desenvolver de forma simples e produtiva, sendo uma linguagem totalmente livre, não somente de custos, mas também de uso, cópia, modificação e distribuição.

Dentre suas diversas características podemos citar:

- Multiplataforma;
- Open source;
- Multiparadigma;
- Tudo é tratado como objeto assim como no [Python](https://www.treinaweb.com.br/blog/afinal-por-que-devo-aprender-python-para-2020/);
- Flexível, uma vez que permite aos seus utilizadores alterar partes da linguagem, sendo assim, partes essenciais do Ruby podem ser removidas ou redefinidas à vontade;
- Utiliza indentação por espaços;
- Não necessita de declarações de variáveis;
- Possui sistema de threading independente do Sistema Operacional, entre outras.

## Aplicações do Ruby

Algumas linguagens de programação podem ser utilizadas para desenvolver qualquer tipo de atividade, mas sabemos que algumas são melhores que outras em determinadas ocasiões. O Ruby não torna-se diferente disso, onde sua utilização pode ser aplicada a diversos usos, como:

- Desenvolvimento web: Para desenvolvimento web, podemos contar com o [framework](https://www.treinaweb.com.br/blog/para-que-serve-um-framework/) Ruby on Rails, que falaremos no próximo artigo. O Ruby on Rails é um framework para desenvolvimento de aplicações web escrito em Ruby. Muito utilizado no mercado, o Ruby on Rails em seus momentos de glória, foi o principal framework web do mundo e até hoje tem uma grande importância no cenário;
- Desenvolvimento desktop: Através do uso das bibliotecas [Shoes](http://shoesrb.com/) e [QtRuby](https://techbase.kde.org/Languages/Ruby), por exemplo, podemos desenvolver aplicações desktop utilizando o Ruby.
- E-commerce: O Ruby é uma ótima linguagem para desenvolvimento também de lojas virtuais. O [Shopify](https://www.shopify.com.br/), por exemplo, é construído utilizando o Ruby.

## Sintaxe

Conhecido por possuir uma sintaxe simples, o Ruby possui algumas características marcantes da linguagem:

- Em Ruby, tudo é um objeto;
- Um cálculo de adição é realizado com o operador mais (+). Mas, se preferir utilizar a palavra escrita `plus`, poderá adicionar esse método à classe nativa `Numeric` do Ruby;
- É possível adicionar uma closure a qualquer método, descrevendo como esse método deve se comportar;
- O Ruby não necessita de declarações de variáveis. Usa simples convenções de nomes para denotar o âmbito das variáveis;
- Possui suporte ao uso de Mixins;
- Por ser indentado a espaços, os conjuntos de instruções no Ruby são finalizados com a palavra `end`, entre outras.

No código escrito em Ruby abaixo, podemos visualizar algumas das características que foram citadas acima:

Copiar

```ruby
class OlaMundo
 	def initialize nome #construtor que inicializa a variável nome
		# Armazena o parâmetro em uma variável de instância.
		@nome = nome
	end
 
	# Método que imprime a mensagem junto com o nome.
	def ola
		puts "Olá, #{@nome}!"
	end
end
 
# Instancia a classe enviando o nome como argumento para o construtor.
ola_mundo= OlaMundo.new "TreinaWeb"
 
# Invoca o método ola, que imprimirá a mensagem.
ola_mundo.ola
```



![Ruby on Rails - Testes unitários](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/ruby-on-rails.svg)

##### CursoRuby on Rails - Testes unitários

[Conhecer o curso](https://www.treinaweb.com.br/curso/testes-unitarios-em-aplicacoes-rails)

O [download do Ruby](https://www.ruby-lang.org/pt/downloads/) pode ser feito em seu próprio site, onde é possível visualizar toda a sua documentação, sua comunidade, novidades sobre a linguagem de programação e muito mais!