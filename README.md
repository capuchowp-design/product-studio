# Product Studio Video — PWA

## Arquivos
- `index.html`: aplicação completa, com HTML/CSS/JavaScript nativos.
- `manifest.webmanifest`: metadados de instalação PWA.
- `sw.js`: cache offline do app shell.
- `icons/`: ícones PNG de 192, 512, maskable e Apple Touch.

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
