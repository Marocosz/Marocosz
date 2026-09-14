Branch de saida do `.github/workflows/metrics.yml` (que vive na `main`).

Ela existe separada da `output` por um motivo concreto: a `output` e publicada
pelo `pacman.yml` com `crazy-max/ghaction-github-pages`, que faz deploy LIMPO —
substitui todo o conteudo da branch pelo `dist/` dele. Em 2026-09-14 isso apagou
duas vezes os SVGs do metrics que estavam la. Essa action nao tem `keep_files`,
entao a unica separacao confiavel e a branch.

Nada aqui e escrito a mao. O README do perfil le estes arquivos por raw.githubusercontent.
