Treino · Registo e Evolução
App web para registar treinos de ginásio: plano Upper/Lower de 4 dias, ilustração de cada exercício, cronómetro de descanso, sugestão automática de carga e relatório mensal.

Não tem servidor nem contas. Os treinos ficam guardados no browser do teu dispositivo (localStorage) e sais quando quiseres com o botão de exportar backup.
Ficheiros
Ficheiro
Para que serve
index.html
A app inteira (HTML + CSS + JS num só ficheiro)
manifest.webmanifest
Nome, cores e ícones para instalar como app
sw.js
Service worker: faz a app funcionar offline
icon-192.png, icon-512.png, icon-maskable-512.png, apple-touch-icon.png
Ícones



Publicar no GitHub Pages
Dá um endereço https fixo, grátis, do tipo https://micaelciencia.github.io/treino/.
1. Criar o repositório
Entra em github.com e faz login.
Canto superior direito → + → New repository.
Repository name: treino
Escolhe Public e carrega em Create repository.

Público? Sim — o GitHub Pages só é grátis em repositórios públicos. O que fica público é apenas o código da app; os teus treinos nunca saem do teu telemóvel, não são enviados para o GitHub. (Pages a partir de repositório privado exige plano pago.)
2. Carregar os ficheiros (sem instalar nada)
No repositório vazio, clica em uploading an existing file (ou Add file → Upload files).
Arrasta para lá todos os ficheiros desta pasta — index.html, manifest.webmanifest, sw.js e os 4 .png. O README.md é opcional.
Em baixo, carrega em Commit changes.

Alternativa por terminal (se preferires git) cd caminho/para/treino-app

git init

git add .

git commit -m "App de treino"

git branch -M main

git remote add origin https://github.com/micaelciencia/treino.git

git push -u origin main
3. Ativar o Pages
No repositório: Settings (menu de cima) → Pages (menu da esquerda).
Em Build and deployment → Source: Deploy from a branch.
Branch: main · pasta / (root) → Save.
Espera 1–2 minutos e recarrega a página: aparece o link https://micaelciencia.github.io/treino/.
4. Instalar no telemóvel
Abre esse link no telemóvel e:

iPhone (Safari): botão de partilha → Adicionar ao ecrã principal. Tem de ser no Safari — no Chrome do iPhone a opção não existe.
Android (Chrome): menu ⋮ → Instalar aplicação / Adicionar ao ecrã principal.

Fica com ícone próprio, abre em ecrã inteiro sem barra do browser e funciona sem rede — podes treinar em caves sem sinal.
5. Passar os treinos que já tens
Os dados estão presos ao endereço onde a app corre, por isso o ficheiro local e o site são "sítios" diferentes. Para levar o histórico contigo:

Abre a versão antiga (o ficheiro no computador) → ícone da base de dados → Exportar backup.
Abre o site novo → ícone da base de dados → Importar backup → escolhe o .json.

Faz o mesmo sempre que quiseres passar de um telemóvel para outro.


Atualizar a app mais tarde
No GitHub: entra em index.html → ícone do lápis (Edit) → cola a versão nova → Commit changes. Em 1–2 minutos está online.

Da próxima vez que abrires a app com internet, aparece em baixo "Nova versão disponível → Atualizar". Os teus treinos não se perdem com a atualização.

Se por algum motivo ficar preso a uma versão antiga: fecha a app, reabre com internet, ou no browser limpa os dados do site só se tiveres feito backup primeiro (limpar os dados do site apaga também os treinos).


Perguntas rápidas
Preciso de pagar alguma coisa? Não. Repositório público + GitHub Pages são grátis.

E se apagar a app do telemóvel? Os dados vão com ela. Exporta o backup de vez em quando — o ficheiro .json é pequeno e podes guardá-lo onde quiseres.

Dá para usar em dois dispositivos ao mesmo tempo? Cada um guarda os seus dados; não há sincronização automática. Passas os dados manualmente por exportar/importar.

Posso mudar o endereço? Sim: muda o nome do repositório, ou usa um domínio próprio em Settings → Pages → Custom domain.

