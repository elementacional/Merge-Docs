# Unificador de Documentos

Aplicação web client-side para mesclar arquivos **DOCX** ou **PDF** diretamente no navegador.

## GitHub Pages

O projeto foi estruturado para funcionar como um site estático no GitHub Pages.

### Estrutura

```text
/
├── index.html
└── README.md
```

### Publicação

1. Crie um repositório no GitHub.
2. Envie `index.html` e `README.md` para a raiz do repositório.
3. Abra **Settings → Pages**.
4. Em **Build and deployment**, selecione:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
5. Salve.
6. Aguarde a publicação e abra o endereço fornecido pelo GitHub Pages.

## Funcionamento

- Seleção manual de arquivos.
- Arrastar e soltar.
- Reordenação dos documentos.
- Mesclagem de DOCX.
- Mesclagem de PDF.
- Download do arquivo resultante.
- Processamento no navegador, sem envio dos documentos para um servidor próprio.

## Bibliotecas

As bibliotecas são carregadas por CDN:

- Tailwind CSS
- JSZip
- pdf-lib
- SortableJS

> Observação: a mesclagem de DOCX é uma operação estrutural sobre o XML interno do arquivo DOCX. Documentos DOCX com estruturas muito complexas, cabeçalhos/rodapés distintos, numeração avançada ou relações internas específicas podem exigir uma estratégia de mesclagem mais sofisticada.
