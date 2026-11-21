[English](../../README.md) | [Português (Brasil)](docs/user/README.pt-BR.md) | [Español](docs/user/README.es.md) | [Català](docs/user/README.ca.md) | [Italiano](docs/user/README.it.md) | [简体中文](docs/user/README.zh-CN.md) | [Русский](docs/user/README.ru.md) | [Bahasa Indonesia](docs/user/README.id.md) | [Polski](docs/user/README.pl.md) | [日本語](docs/user/README.ja.md) | [العربية](docs/user/README.ar.md) | [Ελληνικά](docs/user/README.el.md) | [Türkçe](docs/user/README.tr.md) | **Română**

# Despre

Instrument pentru portarea automată a executabilelor pe Linux și Windows.

Varianta care conține doar relinker-ul rulează pe macOS, inclusiv pe Apple silicon.

[**Convertor web**](https://boykopovar.github.io/AnyPS5/) - fișierele rămân pe dispozitivul tău.

![anyps5_collage1](https://github.com/user-attachments/assets/ed2f0b2d-33d3-46d7-ab88-767ca872fc99)

Include un [relinker](core/relinker) care convertește executabilul în formatul nativ al sistemului țintă, precum și implementări ale [bibliotecilor de sistem prx](core/libs/prx) potrivite pentru legarea dinamică. Fără emulare și fără un proces runtime separat.

[**Discord**](https://discord.gg/x9naWVzC6A), [Utilizare](docs/user/USAGE.md), [Instrucțiuni de compilare](docs/dev/BUILD.md), [Arhitectură](docs/dev/ARCHITECTURE.md), [Datoria tehnică a proiectului](docs/dev/TechnicalDebt.md), [convenții de stil al codului](docs/dev/CONVENTIONS.md), [contribuții](CONTRIBUTING.md)

## Stare

[![libraries](https://boykopovar.github.io/AnyPS5/badge-libraries.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![RDNA2 reference shader forms decoded](https://boykopovar.github.io/AnyPS5/badge-shaders.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![gfx1013 reference shader forms decoded](https://boykopovar.github.io/AnyPS5/badge-shaders-gfx1013.svg)](https://boykopovar.github.io/AnyPS5/progress.html) [![implemented in 7 days](https://boykopovar.github.io/AnyPS5/badge-week.svg)](https://boykopovar.github.io/AnyPS5/history.html)

[![progress map](https://boykopovar.github.io/AnyPS5/progress.svg)](https://boykopovar.github.io/AnyPS5/progress.html)

[Istoricul progresului](https://boykopovar.github.io/AnyPS5/history.html)

<sub>* Biblioteci de sistem: procentul funcțiilor cunoscute de proiect până acum (declarate în [core/libs/prx](core/libs/prx)), nu al tuturor funcțiilor de sistem ale PS5. Totalul crește pe măsură ce sunt declarate mai multe funcții.</sub>

Stările neacceptate sau neașteptate generează o excepție C++, de obicei `std::runtime_error`. O excepție care nu este prinsă de nimic își afișează `what()` pe stderr și încheie procesul.

[Recompilatorul de shadere](core/shader/recompiler/Recompiler.cpp) produce cu succes SPIR-V (validat prin [Spirv-Tools](3rdparty/SPIRV-Tools) atunci când este compilat cu `ANYPS5_ENABLE_SPIRV_TOOLS`).

## Compatibilitate

Starea fiecărui joc și rapoartele de testare se găsesc în discuțiile [Game bring-up](https://github.com/boykopovar/AnyPS5/discussions/categories/game-bring-up), câte un fir pentru fiecare titlu.

## Maparea intrărilor

Controllerele de joc mapate prin SDL sunt acceptate, inclusiv stick-urile analogice și trigger-ele. Controalele de tastatură și mouse pot fi configurate printr-un fișier `anyps5-input.ini`. Consultă [maparea intrărilor](docs/user/INPUT_MAPPING.md) pentru dispozitivele acceptate și formatul de configurare.

## Declinarea responsabilității

Acest proiect este destinat interoperabilității, cercetării, conservării și compatibilității. Nu include, nu distribuie și nu necesită software protejat de drepturi de autor, firmware, chei criptografice sau biblioteci proprietare. Utilizatorii sunt responsabili să se asigure că orice binare folosite cu acest proiect sunt obținute și utilizate în conformitate cu legile aplicabile și cu termenii de licență respectivi.

AnyPS5 este un proiect independent și nu este afiliat cu Sony Interactive Entertainment, nici autorizat sau susținut de aceasta. „PlayStation” și „PS5” sunt mărci comerciale ale Sony Interactive Entertainment Inc.

## Licență

Acest proiect este licențiat sub GNU General Public License versiunea 2 exclusiv.
