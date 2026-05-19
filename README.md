# 🏎 BI Drives

Dashboard de análise de drives — importa planilhas diárias, acumula histórico e filtra por dia.

## Como usar

1. Acesse o dashboard via GitHub Pages: `https://SEU_USUARIO.github.io/bi-drives`
2. Selecione a **data** do dia
3. Faça **upload** da planilha `.xlsx` do dia
4. Clique em **PROCESSAR E SALVAR**
5. Use os chips de **filtro por dia** para comparar datas

## Estrutura esperada da planilha

A planilha deve seguir o formato padrão com seções de carros lado a lado, cada seção contendo as colunas:
- **Coluna B (offset 1)**: Nome do cliente
- **Coluna D (offset 3)**: Vendedor
- **Coluna F (offset 5)**: C/D (Drive ou Carona)
- **Coluna K (offset 10)**: Instrutor
- **Coluna O (offset 14)**: Status

Carros suportados: Mustang Black, Mustang White, Mustang Red, 718, Porsche 911 Carrera, Maserati GranCabrio, Camaro Bordo, Mustang 2025, Ferrari California, Shelby GT-500, Corvette C6, BMW M3, McLaren 600LT, Ferrari Portofino, Lamborghini Gallardo, Corvette C7.

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub (ex: `bi-drives`)
2. Faça upload do arquivo `index.html`
3. Vá em **Settings → Pages**
4. Em "Source", selecione `main` branch e pasta `/ (root)`
5. Clique em **Save** — o link estará disponível em instantes

## Dados

Os dados ficam salvos no **localStorage** do navegador (por dispositivo). Para compartilhar entre dispositivos, use o mesmo navegador logado ou exporte/importe os dados manualmente.

## Tecnologias

- HTML/CSS/JS puro — sem dependências de servidor
- [SheetJS](https://sheetjs.com/) — leitura de arquivos Excel
- [Chart.js](https://chartjs.org/) — gráficos interativos
- GitHub Pages — hospedagem gratuita
