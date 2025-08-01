### Quick Start (Local Version) 🚀



1. Install pnpm if you don't have it


```
npm install -g pnpm
```

2. Install the dApp

```bash
pnpm i
```

3. Create the Database 

(Optional) Start a local PostgreSQL instance

If you already have your own PostgreSQL running, you can skip this step.

In that case, make sure to update the PostgreSQL URL in your .env file.

```
pnpm docker:pg-chatzero
```

This create a Postgres DB here:
```
POSTGRES_URL=postgres://zero:group@localhost:5432/chat
```

4. Fill the .env file

Enter required information in the .env file

The .env file is created automatically. Just fill in the required values.

For the fastest setup, provide at least one LLM provider's API key (e.g., OPENAI_API_KEY, CLAUDE_API_KEY, GEMINI_API_KEY, etc.) and the PostgreSQL URL you want to use.

5. Migrate the DB

```sh
pnpm db:migrate
```

5. Build 

```
pnpm build:local 
```

6. Start

```
pnpm start
```



# Errore

ReferenceError: localStorage is not defined
    at <unknown> (C:\Projects\Radix\ZeroCollateral\chatxrd\.next\server\chunks\5249.js:1:53563)
    at t.a (C:\Projects\Radix\ZeroCollateral\chatxrd\.next\server\webpack-runtime.js:1:891)
    at 86120 (C:\Projects\Radix\ZeroCollateral\chatxrd\.next\server\chunks\5249.js:1:52949)
    at Function.t (C:\Projects\Radix\ZeroCollateral\chatxrd\.next\server\webpack-runtime.js:1:128)