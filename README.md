# Festival Raízes Originárias — site oficial

Landing page estática (HTML + CSS + um pouco de JS), sem dependências externas.
Hospedagem: GitHub Pages · Domínio: **festivalraizesoriginarias.com.br**

## Estrutura

```
index.html                 → o site inteiro (HTML, CSS e JS no mesmo arquivo)
CNAME                      → domínio personalizado (não apague)
.nojekyll                  → evita que o GitHub processe o site como Jekyll
favicon.ico
assets/img/                → imagens usadas no site (fundo transparente)
assets/marca/              → arquivos originais da identidade visual (backup)
```

## Paleta oficial

| Cor      | Hex       |
|----------|-----------|
| Marrom   | `#381c0f` |
| Amarelo  | `#f6b20a` |
| Vermelho | `#770706` |
| Verde    | `#00a18e` |
| Branco   | `#ffffff` |

Tipografia: Helvetica Neue / Helvetica / Arial (fontes do sistema, sem carregamento externo).

## Publicar no GitHub Pages

1. Crie um repositório público (ex.: `festival-raizes-originarias`).
2. Envie **todo o conteúdo desta pasta** para a raiz do repositório (o `index.html` precisa ficar na raiz).
3. Em **Settings → Pages**, escolha *Deploy from a branch* → branch `main` → pasta `/ (root)` → **Save**.
4. Ainda em **Settings → Pages**, campo **Custom domain**, digite `festivalraizesoriginarias.com.br` e salve.
5. Marque **Enforce HTTPS** (pode levar alguns minutos até liberar).

## DNS no registrador do domínio

Domínio raiz (`@`) — quatro registros **A**:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Opcional (IPv6) — quatro registros **AAAA**:

```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

Subdomínio `www` — um registro **CNAME** apontando para `SEU-USUARIO.github.io`

A propagação pode levar de alguns minutos até 24 horas.

## Editar o conteúdo

Todo o texto está em `index.html`, em português, dentro de seções comentadas
(`HERO`, `O FESTIVAL`, `O QUE FAZEMOS`, `QUEM CELEBRAMOS`, `MANIFESTO`, `CONTATO`).
As cores estão centralizadas no bloco `:root` do `<style>`.
