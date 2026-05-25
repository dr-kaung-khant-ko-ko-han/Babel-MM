What is this document about? This user guide focuses on internationalization and localization with LATEX and luatex, pdftex and xetex with the babel package. There are also some notes on its use with e-Plain and pdf-Plain TEX. 

I only need learn the most basic features. The first subsections (1.1-1.6) describe the ways of loading a language, which is usually all you need. 

I don’t like manuals. I prefer sample files. This manual contains lots of examples and tips, but in GitHub there are many sample files. 

What if I’m interested only in the latest changes? Changes and new features with relation to version 3.8 are highlighted with X.XX (※ is a link to the babel site), and there are some notes for the latest versions in the babel site. The most recent features can still be unstable. Remember version 24.1 follows 3.99, because of a new numbering scheme. 

Can I help? Sure! You can follow the development of babel in GitHub and make suggestions, including requirements for some language or script. Feel free to fork it and make pull requests. If you are the author of a package, send me a few test files which I’ll add to mine, so that possible issues can be caught in the development phase. 

It doesn’t work for me! You can ask for help in some forums like tex.stackexchange, but if you have found a bug, I strongly beg you to report it in GitHub, which is much better than just complaining on an e-mail list or a web forum. Remember warnings are not errors by themselves, they just warn about possible problems or incompatibilities. Hyphenation rules are maintained separately here. 

How can I contribute a new language? See section 9.1 for contributing a language. 

Where is the code? Run lualatex--jobname=babel-code \let\babelcode\relax\input{babel.dtx}. 

NOTE Now that the recommend engine for LATEX is luatex, you can read Migrating from pdfTeX to LuaTeX and Migrating from XeTeX to LuaTeX.