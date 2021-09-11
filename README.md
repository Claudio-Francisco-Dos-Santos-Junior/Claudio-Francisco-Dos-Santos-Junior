# 🤚 Olá humano, meu nome é Cláudio!
- 👀 I’m interested entender e compreender o mundo da programação e da tecnologia.

<blockquote>

> “Uma máquina consegue fazer o trabalho de 50 homens ordinários. Nenhuma máquina consegue fazer o trabalho de um homem extraordinário”.

<!---
Claudio-Francisco-Dos-Santos-Junior/Claudio-Francisco-Dos-Santos-Junior is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
  
  [![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Claudio-Francisco-Dos-Santos-Junior)](https://github.com/Claudio-Francisco-Dos-Santos-Junior/github-readme-stats)

  ### Procuro sempre estar atualizado e futuramente quero abrir minha própria marca de produtos tecnológicos.
  
  [![Claudio's GitHub stats](https://github-readme-stats.vercel.app/api?username=Claudio-Francisco-Dos-Santos-Junior)](https://github.com/Claudio-Francisco-Dos-Santos-Junior/github-readme-stats)

 -----------------------------------------------------------------------------------
  
  nome: Gerar Dados

em:
  horário:  # executar a cada 12 horas
    - cron:  "* */12 * * *" 
  workflow_dispatch:

empregos:
  construir:
    nome: Empregos para atualizar dados
    runs-on: ubuntu-latest
    passos:
      # Animação cobra
      - usos: Platane/snk@master
        id: snake-gif
        com:
          github_user_name: joevtap
          svg_out_path: dist/github-contribution-grid-snake.svg

      - usa: crazy-max/ghaction-github-pages@v2.1.3
        com:
          target_branch: saída
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{{ segredos. GITHUB_TOKEN }}
