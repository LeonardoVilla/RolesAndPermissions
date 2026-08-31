# Roles and Permissions

CRUD de controle de acesso (RBAC) em Laravel usando
[spatie/laravel-permission](https://spatie.be/docs/laravel-permission), com
frontend em React via Inertia.js.

## O que tem

- **Roles e Permissions** com CRUD completo (`RoleController`,
  `UserController`) — atribuição de múltiplas permissões por papel.
- Middleware de permissão granular por rota (`role-list`, `role-create`,
  `role-edit`, `role-delete`), aplicado no construtor dos controllers.
- Módulo de exemplo (`Product`) protegido pelas mesmas permissões, pra
  mostrar o RBAC funcionando sobre um recurso de negócio real e não só nas
  telas de administração.

## Stack

Laravel · Inertia.js + React + TypeScript · Radix UI + Tailwind CSS ·
spatie/laravel-permission

## Rodando localmente

```bash
composer install
npm install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
npm run dev
```
