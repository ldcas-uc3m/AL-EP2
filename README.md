# Ejercicio Práctico 2
By Luis Daniel Casais Mezquida & Diego Picazo García  
Aspectos Legales y Éticos de la Ingeniería Informática 24/25  
Máster en Ingeniería Informática  
Universidad Carlos III de Madrid


## Enunciado de la práctica
El trabajo deberá evidenciar una empresa española que, en el momento de redactar el trabajo, incumpla, de alguna forma y en alguna medida, lo dispuesto en la normativa de Servicios de la Sociedad de la Información ([LSSICE](https://www.boe.es/eli/es/l/2002/07/11/34/con)), justificando pormenorizadamente el presunto o presuntos incumplimientos, el precepto o preceptos supuestamente incumplidos, su ubicación en la citada normativa y las presuntas consecuencias de tal incumplimiento.



## Compilation
This report follows [GUL's UC3M LaTeX report template](https://github.com/guluc3m/report-template/). More information and updated versions on the original repository.

First you must install [LaTeX](https://www.latex-project.org/).

- For Linux, install `texlive-full`.
- For Windows, install [MiKTeX](https://miktex.org/download#win), make sure you add it to your `PATH`, and install [Perl](https://strawberryperl.com/). If it’s not installed already, open the MikTeX Package Manager and install the `latexmk` package.
- For MacOS, install [MacTeX](https://www.tug.org/mactex/mactex-download.html) and then install `latexmk` with:
    ```
    sudo tlmgr install latexmk
    ```

> [!IMPORTANT]
> As we'll use SVG files, you'll need to install [Inkscape](https://inkscape.org/).
> If you're in Windows, make sure to add the executable to your PATH (typically located in `C:\Program Files\Inkscape\bin\`).

To compile the report, use the command:
```
latexmk -cd -shell-escape -pdf report.tex
```

## VS Code
Some useful extensions:
- [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)
> [!IMPORTANT]
> If you are using the extension, please set `-shell-escape` (see [LaTeX Workshop FAQ](https://github.com/James-Yu/LaTeX-Workshop/wiki/FAQ#how-to-pass--shell-escape-to-latexmk))

> [!TIP]
> You can enable the wordcount by setting `latex-workshop.wordcount` to `onSave` in the settings. More information [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/ExtraFeatures#counting-words)
- [LTeX+](https://marketplace.visualstudio.com/items?itemName=ltex-plus.vscode-ltex-plus): Grammar checker.
> [!TIP]
> You can change the language through the `ltex.language` setting in VS Code settings.
