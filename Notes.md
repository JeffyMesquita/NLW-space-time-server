## Start Backend Project in NodeJs

### 1. Create a new folder for the project

```bash
mkdir server
```

### 2. Create a new package.json file

```bash
npm init -y
```

### 3. Install typescript

```bash
npm i typescript @types/node -D
```

### 4. Create a new tsconfig.json file

```bash
npx tsc --init
```

### 5. In tsconfig.json file, change target

```bash
"target": "es2020",
```

### 6. Create src folder

```bash
mkdir src
```

### 7. Create server.ts file

```bash
touch src/server.ts
```

### 8. Install tsx

```bash
npm i tsx -D
```

### 9. In package.json file, add scripts

```bash
"scripts": {
    "dev": "tsx watch src/server.ts"
  },
```

### 10. Install fastify

```bash
npm i fastify
```

### 11. Install ESLint

```bash
npm i eslint -D
```

### 12. Install ESLint Rocketseat

```bash
npm i @rocketseat/eslint-config -D
```

### 13. Create .eslintrc.json file

```bash
touch .eslintrc.json
```

### 14. In .eslintrc.json file, add

```bash
{
  "extends": [
    "@rocketseat/eslint-config/node"
  ]
}
```

### 15. In package.json file, add scripts

```bash
"scripts": {
    "dev": "tsx watch src/server.ts",
    "lint": "eslint --fix src --ext .ts"
  },
```

### 16. Install Prisma

```bash
npm i prisma -D
```


### 17. Initialize Prisma

```bash
npx prisma init --datasource-provider SQLite
```

### 18. Run Migrations

```bash
npx prisma migrate dev
```

### 19. Install Prisma Client

```bash
npm i @prisma/client
```
