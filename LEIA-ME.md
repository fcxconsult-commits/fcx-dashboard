# 📊 FCX Dashboard Marketing 2026

## 📁 Estrutura de arquivos

```
fcx-dashboard/
├── index.html        ← Dashboard (abra este no navegador)
├── dados_fcx.csv     ← Dados das tarefas (EDITE ESTE para atualizar)
└── LEIA-ME.md        ← Este guia
```

---

## 🔄 Como atualizar os dados

### Opção A — Pelo próprio dashboard (mais fácil)
1. Abra o `index.html` no navegador
2. Clique em **"📂 Selecionar novo CSV"** no banner azul do topo
3. Selecione seu arquivo CSV atualizado
4. O dashboard atualiza **na hora**, sem recarregar a página

### Opção B — Substituindo o arquivo CSV
1. Edite o arquivo `dados_fcx.csv` (Excel, Google Sheets, ou bloco de notas)
2. Salve com o mesmo nome `dados_fcx.csv`
3. Recarregue o dashboard no navegador

---

## 📋 Formato do CSV

O arquivo `dados_fcx.csv` deve ter **exatamente estas colunas** (a ordem não importa):

| Coluna | Exemplo | Descrição |
|---|---|---|
| `num` | `1` | Número sequencial da tarefa |
| `canal` | `INSTAGRAM` | Canal de marketing |
| `marca` | `FCX CONSULTORIA` | Marca/subcategoria |
| `tarefa` | `Bio — descrição do perfil` | Nome da tarefa |
| `obs` | `Texto, link e emojis` | Observações (opcional) |
| `resp` | `Ronaldo F.` | Responsável |
| `progresso` | `0.9` | Progresso de 0 a 1 (ex: 0.9 = 90%) |
| `inicio` | `02/03/2026` | Data de início (DD/MM/AAAA) |
| `termino` | `13/03/2026` | Data de término (DD/MM/AAAA) |

### Valores de progresso:
- `0` → Não iniciado
- `0.1` a `0.9` → Em andamento
- `1` → Concluído

---

## 🌐 Publicar no GitHub Pages (atualização automática)

### Primeira vez (5 minutos):
1. Crie uma conta gratuita em **github.com**
2. Clique em **"New repository"** → nome: `fcx-dashboard` → marque **Public** → clique em **Create**
3. Arraste os 3 arquivos (`index.html`, `dados_fcx.csv`, `LEIA-ME.md`) para a página do repositório
4. Vá em **Settings → Pages → Branch: main → Save**
5. Aguarde ~1 minuto → seu dashboard estará em:
   **`https://seuusuario.github.io/fcx-dashboard`**

### Para atualizar depois:
1. Acesse seu repositório no GitHub
2. Clique em `dados_fcx.csv` → ícone de lápis (editar)
3. Faça as alterações → clique **"Commit changes"**
4. O dashboard atualiza automaticamente em ~30 segundos ✅

---

## 💡 Dicas

- **Novas tarefas:** adicione novas linhas no CSV mantendo o formato
- **Novo canal:** basta digitar o nome — o dashboard detecta automaticamente
- **Progresso:** atualize o campo `progresso` conforme as tarefas avançam
- O campo `mes` é calculado automaticamente pelas datas de início e fim

