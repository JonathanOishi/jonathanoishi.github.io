# Jonathan Oishi — Portfólio

Portfólio pessoal desenvolvido em **Flutter Web**, projetado para apresentar minha trajetória profissional, competências técnicas e projetos de forma moderna, responsiva e escalável.

🔗 **Site no ar:** [jonathanoishi.github.io](https://jonathanoishi.github.io)

<p align="center">
  <a href="https://github.com/JonathanOishi">
    <img
      src="https://i.ibb.co/1Y2tnP11/Chat-GPT-Image-17-de-jun-de-2026-08-16-24-removebg-preview.png"
      alt="Geo Tasks"
      width="60%"
    />
  </a>
</p>

O objetivo deste projeto foi construir uma aplicação web com foco em performance, organização arquitetural e experiência do usuário, utilizando boas práticas de desenvolvimento e uma estrutura preparada para futuras evoluções.

## Sobre o Projeto

Este portfólio centraliza minha apresentação profissional em uma única plataforma, permitindo que recrutadores, empresas e parceiros conheçam minha experiência, formação e principais projetos.

A aplicação foi construída em Flutter Web e segue uma arquitetura modular baseada em componentes reutilizáveis, facilitando manutenção, expansão e escalabilidade. O deploy é automatizado via GitHub Actions, publicando diretamente no GitHub Pages a cada push na branch `master`.

## Principais Seções

* Apresentação inicial (Hero Section), com fundo animado de partículas
* Minha trajetória (Sobre Mim / História)
* Stack tecnológica, organizada por categorias com nível de domínio
* Experiência profissional
* Formação acadêmica
* Projetos em destaque (MyFinancy, GeoTasks e este próprio portfólio)
* Orçamentos e serviços
* Contato, com formulário que envia a mensagem direto para o WhatsApp e botão de download do currículo
* Rodapé institucional, com atalho para voltar ao topo

A navegação principal é feita por uma barra fixa (desktop/tablet) ou por um drawer lateral (mobile), com rolagem suave até cada seção.

## Tecnologias Utilizadas

* **Flutter** / **Dart**
* **Material Design 3**
* `url_launcher` — abertura de links externos (LinkedIn, GitHub, WhatsApp, currículo)
* `flutter_launcher_icons` — geração automática dos ícones da aplicação web
* **GitHub Actions** — pipeline de build e deploy contínuo
* **GitHub Pages** — hospedagem do site

## Arquitetura

O projeto foi estruturado seguindo princípios de organização e separação de responsabilidades.

```text
lib/
├── core/
│   ├── responsive/      # Breakpoints, tipos de dispositivo e utilitários de responsividade
│   ├── scroll/           # Comportamento de scroll customizado (suporte a mouse/trackpad)
│   ├── services/         # Integrações externas (ex.: WhatsApp)
│   └── theme/            # Cores, tipografia e tema centralizado (Design System)
│
├── features/
│   ├── animation/         # Animações reutilizáveis (ex.: blinking dot)
│   └── view/
│       ├── navigation/    # Itens e identificadores das seções de navegação
│       ├── pages/         # HomePage — orquestra todas as seções
│       ├── sections/      # Hero, História, Stack, Experiência, Educação, Projetos, Serviços, Contato, Footer
│       └── widgets/        # Navbar, drawer mobile e efeito de partículas
│
└── main.dart              # Ponto de entrada da aplicação
```

### Destaques da Arquitetura

* Componentização de widgets
* Estrutura baseada em features
* Responsividade centralizada (mobile, tablet e desktop)
* Design System unificado
* Fácil manutenção e expansão
* Separação clara entre regras visuais e lógica de apresentação

## Design System

Todo o sistema visual foi centralizado para garantir consistência em toda a aplicação.

### AppColors

Todas as cores do projeto são gerenciadas através da classe `AppColors`, eliminando valores hardcoded e facilitando futuras alterações de identidade visual.

### Tipografia e Espaçamento

Os estilos de texto e os espaçamentos seguem padrões centralizados (`AppTextStyle` e `AppSpacing`), reutilizados em todas as seções para manter consistência visual.

### Responsividade

A adaptação entre mobile, tablet e desktop é realizada através de utilitários centralizados em `core/responsive`, garantindo uma experiência consistente em diferentes tamanhos de tela — incluindo grids que se reorganizam em colunas, carrossel em mobile para os cards de projeto e tipografia fluida.

## Diferenciais do Projeto

* Layout moderno e responsivo
* Navegação fluida entre seções com rolagem animada
* Drawer mobile integrado à navegação principal
* Fundo animado com efeito de partículas na Hero Section
* Formulário de contato integrado ao WhatsApp
* Código organizado e escalável
* Componentes reutilizáveis
* CI/CD configurado para deploy automático
* Estrutura preparada para crescimento contínuo
* Foco em legibilidade e manutenção

## Evolução Contínua

Este projeto continuará recebendo melhorias e novas funcionalidades conforme minha evolução profissional e tecnológica.

## Autor

### Jonathan Oishi

Desenvolvedor Flutter especializado em aplicações mobile e web, com foco em arquitetura limpa, interfaces modernas e experiências digitais escaláveis.

* [LinkedIn](https://www.linkedin.com/in/jonathanoishi/)
* [GitHub](https://github.com/JonathanOishi)
