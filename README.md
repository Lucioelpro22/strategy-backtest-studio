# Strategy Backtest Studio

Constructor visual de estrategias de trading que genera código Python compatible con [Backtrader](https://www.backtrader.com/).

## Demo

[Abrir Strategy Backtest Studio](https://strategy-backtest-studio.lucianohernanleal22.chatgpt.site)

## Funcionalidades

- Constructor visual de reglas de entrada y salida.
- Indicadores SMA, EMA, RSI y MACD.
- Stop loss y take profit configurables.
- Validación y preflight antes de exportar.
- Configuración de capital, comisión y tamaño de posición.
- Vista previa y exportación de una estrategia `.py`.
- Exportación de la configuración en JSON.
- Autoguardado local en el navegador.
- Código generado con manejo de órdenes y analizadores de Backtrader.
- Motor de backtesting en el navegador, sin enviar datos a servidores.
- Importación de CSV OHLCV y dataset demo incluido.
- Curva de capital, retorno, drawdown, win rate y profit factor.
- Tabla de operaciones y exportación de resultados en CSV.

## Desarrollo local

Es una aplicación estática sin dependencias de compilación. Podés servir el directorio `dist` con cualquier servidor HTTP:

```bash
python -m http.server 8000 --directory dist
```

Luego abrí `http://localhost:8000`.

## Estructura

```text
dist/
├── index.html
├── styles.css
├── professional.css
├── backtest.css
├── app.js
└── backtest.js
```

## Alcance

La aplicación incluye una simulación local para validar ideas rápidamente. Para investigación cuantitativa de producción, el archivo Python exportado debe ejecutarse con un `data feed` de Backtrader y contemplar slippage, calidad de datos y sesgos del mercado.


