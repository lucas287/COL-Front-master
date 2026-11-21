# COL — Controle Operacional Lógico | Frontend

Aplicação web de gestão operacional desenvolvida com React, TypeScript e Vite. Este repositório contém a interface do sistema; a API fica no repositório [COL-BACK](https://github.com/lucas287/COL-BACK).

## Tecnologias

- React 18
- TypeScript
- Vite
- Tailwind CSS e componentes Radix/shadcn
- React Router
- TanStack Query
- Socket.IO Client

## Módulos presentes no frontend

- Dashboard e indicadores
- Produtos e estoque
- Solicitações, separações e reposições
- Relatórios e cálculos
- Tarefas, lembretes e rotinas de escritório
- Usuários, permissões e auditoria
- Autenticação e notificações

## Executar localmente

```bash
npm install
npm run dev
```

Para validar a compilação:

```bash
npm run build
```

## Configuração da API

O frontend lê a variável de ambiente `VITE_API_URL` para definir a URL do backend. Em produção, configure essa variável com o endereço HTTPS real da API. Sem ela, o código usa um endereço local/de fallback que não é adequado para uma implantação pública.

O backend também precisa permitir a origem pública do frontend na configuração de CORS. O endereço de produção e a integração entre frontend e API devem ser testados antes de divulgar a aplicação.

Crie um arquivo local `.env.local` para a configuração do ambiente e não publique credenciais ou tokens no Git.

## Backend

[Repositório COL-BACK](https://github.com/lucas287/COL-BACK)

## Status de publicação

O código está no GitHub. Uma demonstração pública só deve ser divulgada depois de configurar a URL da API, o CORS e validar login, dados e comunicação em tempo real.
