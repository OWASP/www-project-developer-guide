---

title: Design
layout: col-document
tags: Guia do Desenvolvedor do OWASP
contributors:
document: Guia do Desenvolvedor do OWASP
order:

---

{% include breadcrumb.html %}

![WIP logo](../../../assets/images/dg_wip.png "Trabalho em andamento"){height=180px}

## 4. Design

Não há tradução para esta página, consulte a [versão original em inglês][release0600].

Sections:

4.1 [Modelagem de ameaças](#modelagem-de-ameaças)  
4.1.1 [Modelagem de ameaças na prática](#modelagem-de-ameaças-na-prática)  
4.1.2 [pytm](#pytm)  
4.1.3 [Threat Dragon](#threat-dragon)  
4.1.4 [Cornucopia](#cornucopia)  
4.1.5 [LINDDUN GO](#linddun-go)  
4.1.6 [Toolkit para Modelagem de Ameaças](#toolkit-para-modelagem-de-ameaças)  
4.2 [Lista de verificação para aplicação web](#lista-de-verificação-para-aplicação-web)  
4.2.1 [Defina Requisitos de Segurança](#defina-requisitos-de-segurança)  
4.2.2 [Utilize Frameworks e Bibliotecas de Segurança](#utilize-frameworks-e-bibliotecas-de-segurança)  
4.2.3 [Proteja Acesso ao Banco de Dados](#proteja-acesso-ao-banco-de-dados)  
4.2.4 [Codifique e Escape Dados](#codifique-e-escape-dados)  
4.2.5 [Valide todas as entradas](#valide-todas-as-entradas)  
4.2.6 [Implemente Identidade Digital](#implemente-identidade-digital)  
4.2.7 [Imponha Controles de Acesso](#imponha-controles-de-acesso)  
4.2.8 [Proteja Dados em Todos os Lugares](#proteja-dados-em-todos-os-lugares)  
4.2.9 [Implemente Registro e Monitoramento de Segurança](#implemente-registro-e-monitoramento-de-segurança)  
4.2.10 [Trate todos os Errors e Exceções](#trate todos-os-errors-e-exceções)  
4.3 [MAS Lista de verificação](#mas-lista-de-verificação)  

----

[release0600]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/06-design/toc.md
