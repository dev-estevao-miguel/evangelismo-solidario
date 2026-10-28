# Evangelismo Solidário

Sistema web para ações sociais de igrejas: cadastro rápido da população, confirmação de presença por atividade e resumo dos atendimentos em tempo real.

<p>
  <img alt="Status" src="https://img.shields.io/badge/status-conclu%C3%ADdo%20(demo)-10bfe1?style=flat-square"/>
  <img alt="HTML" src="https://img.shields.io/badge/HTML5-1f2334?style=flat-square&logo=html5&logoColor=E34F26"/>
  <img alt="CSS" src="https://img.shields.io/badge/CSS3-1f2334?style=flat-square&logo=css3&logoColor=1572B6"/>
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-ES%20Modules-1f2334?style=flat-square&logo=javascript&logoColor=F7DF1E"/>
  <img alt="Dados" src="https://img.shields.io/badge/dados-100%25%20fict%C3%ADcios-10bfe1?style=flat-square"/>
</p>

> **Versão de demonstração.** Não há banco de dados nem credenciais reais: tudo o que for digitado fica apenas no navegador de quem testa (localStorage). Marca e imagens da campanha original foram substituídas por elementos genéricos ("Igreja Demo").

## O problema

Em uma ação social, centenas de pessoas passam por várias atividades no mesmo dia: atendimento odontológico, aferição de pressão, orientação jurídica, corte de cabelo, doação de roupas. O controle costuma ser feito em fichas de papel, que se perdem, se repetem e só são somadas dias depois.

Sem um registro único, a organização não sabe quantas pessoas foram atendidas em cada atividade, quem já passou por onde e qual serviço teve mais procura, informações essenciais para prestar contas e planejar a próxima ação.

O Evangelismo Solidário resolve isso com um ID por participante: o voluntário da entrada cadastra a pessoa uma vez, cada atividade confirma a presença pelo ID e a administração acompanha o resumo ao vivo e exporta tudo ao final.

## O que faz

- Cadastro de participantes (nome, idade, telefone e data/hora) com ID gerado automaticamente.
- Confirmação de presença por ID em 11 atividades (odontologia, pressão e glicose, psicologia, roupas, cabelo, estética, jurídico, culto infantil, 2ª via de documentos e faturas, xerox).
- Resumo em tempo real dos atendimentos.
- Administração com busca, edição, exclusão e exportação em CSV.

## Capturas

A interface roda direto no navegador; veja abaixo como abrir a demonstração localmente.

## Stack

HTML · CSS · JavaScript (ES Modules) · LocalStorage.

## Como executar

O `app.js` usa módulos ES; abra o projeto por um servidor estático:

```bash
python -m http.server 8080
```

Acesse http://localhost:8080. Administração (demo): usuário `demo`, senha `demo`.

## Escopo da versão pública

- Versão demonstrativa do sistema usado em uma ação solidária real em 2025.
- A versão original usava um banco na nuvem; esta guarda os dados só no navegador. Nenhum dado de participante foi publicado.
- Logotipo e fundo são genéricos, gerados para a demonstração.

## Licença

[MIT](LICENSE)

---

Desenvolvido por **Estevão Santos** · [github.com/dev-estevao-miguel](https://github.com/dev-estevao-miguel)
