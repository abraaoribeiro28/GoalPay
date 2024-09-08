# GoalPay

**GoalPay** é um sistema de gerenciamento de funcionários e cargos com foco no controle de metas semanais e metas iniciais para novos funcionários. O sistema permite a criação de contas com permissões baseadas em cargos, garantindo que cada usuário tenha acesso apenas às funcionalidades permitidas de acordo com seu nível hierárquico.

## Funcionalidades Principais

- **Gerenciamento de Funcionários:** Adição, edição e remoção de funcionários, com a definição de metas personalizadas.
- **Controle de Metas Semanais:** Acompanhamento do progresso das metas semanais de cada funcionário.
- **Metas Iniciais para Novos Funcionários:** Configuração de metas específicas para novos colaboradores em fase inicial.
- **Sistema de Login com Permissões e Cargos:** Gestão de permissões baseada em cargos para controlar o acesso às funcionalidades do sistema.

## Requisitos

- **PHP:** >= 8.1
- **Composer:** >= 2.x
- **MySQL:** >= 5.7
- **Node.js:** >= 16.x (para compilar os assets)

## Instalação

### Clone do projeto
<p>
    Comece clonando o projeto para o seu local
</p>

```bash
git clone https://github.com/abraaoribeiro28/GoalPay.git
```

### Configurações do projeto
Após clonar o projeto, copie o arquivo `.env.example` nomeando-o para `.env.` <br>
Modifique as informações de conexão do seu banco de dados no arquivo `.env`:

```bash
DB_CONNECTION=sqlite
#DB_HOST=127.0.0.1
#DB_PORT=3306
#DB_DATABASE=laravel
#DB_USERNAME=root
#DB_PASSWORD=
```

Caso você queira continuar com o sqlite, crie um arquivo `databse.sqlite` dentro da pasta `database`.

### Execução
Instale as dependencias do composer com:

```bash
composer install
```
Em seguida execute os seguintes comandos

```bash
php arisan key:generate
php artisan migrate --seed
```
Agora faça o build dos assets

```bash
npm install
npm run build
```
Execute o comando para simular um servidor

```bash
php artisan serve
```
Agora em seu navegador acesse

```bash
localhost:8000
```

Agora o projeto deve estar funcionando.
