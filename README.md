# Product Studio Video — PWA

## Arquivos
- `index.html`: aplicação completa, com HTML/CSS/JavaScript nativos.
- `manifest.webmanifest`: metadados de instalação PWA.
- `sw.js`: cache offline do app shell.
- `icons/`: ícones PNG de 192, 512, maskable e Apple Touch.

## Modos de vídeo
- **Estúdio**: uma foto por vez, com movimento e transições.
- **Feed rolante**: fundo 9:16 desfocado e parado (de uma das fotos ou de outra imagem enviada) com as fotos com cantos arredondados em 4 animações: subindo (contínuo), da direita para a esquerda (contínuo), cubo 3D e página virando.

## Publicar no GitHub Pages
1. Envie todos os arquivos e a pasta `icons/` para a raiz do repositório.
2. Abra **Settings → Pages**, escolha a branch e `/ (root)`.
3. Abra a URL HTTPS publicada no Chrome/Edge.
4. No menu do navegador, escolha **Instalar app** ou **Adicionar à tela inicial**.

## Limitações
- PWA e Service Worker precisam de HTTPS (ou localhost); `file://` abre o editor, mas não instala o PWA.
- MP4 só é exportado se o navegador suportar MediaRecorder com MP4; WebM tem suporte mais amplo.
- Fotos e vídeos são processados no dispositivo. O cache guarda apenas os arquivos estáticos do app.
- Sem IA/biblioteca de segmentação, não é possível remover de forma confiável o fundo já incorporado a uma foto comum.
