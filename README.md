# Site DMT Tech — dmttech.com.br

HTML + CSS puro, sem build. Hospedado no GitHub Pages.

## Estrutura
- `index.html` — página única (desktop e celular)
- `favicon.svg` — ícone da aba
- `CNAME` — domínio dmttech.com.br (não apagar)
- `img/` — fotos dos sócios e logo oficial

## Pendências (fazer depois)
- [ ] WhatsApp: preencher a constante `WHATSAPP` no fim do index.html (o link aparece sozinho)
- [ ] Criar a caixa contato@dmttech.com.br (o formulário envia pra ela enquanto não tiver WhatsApp)
- [ ] Fotos dos sócios em `img/` (trocar os círculos GT / DM)
- [ ] Cargo/especialidade dos sócios, região de atendimento, CNPJ no rodapé

## DNS no registro.br (dmttech.com.br → GitHub Pages)
Painel registro.br → domínio → DNS → Editar zona (usar DNS do Registro.br):

| Tipo  | Nome  | Valor                    |
|-------|-------|--------------------------|
| A     | (vazio/@) | 185.199.108.153     |
| A     | (vazio/@) | 185.199.109.153     |
| A     | (vazio/@) | 185.199.110.153     |
| A     | (vazio/@) | 185.199.111.153     |
| CNAME | www   | SEU-USUARIO.github.io    |

Depois: GitHub → Settings → Pages → Custom domain = dmttech.com.br → Save.
Quando o check ficar verde, marcar **Enforce HTTPS**.
