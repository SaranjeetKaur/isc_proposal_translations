# isc-proposal

## Consistent Translations Glossary across R

[![build-status](https://github.com/SaranjeetKaur/isc_proposal_translations/actions/workflows/publish-proposal.yaml/badge.svg)](https://github.com/SaranjeetKaur/isc_proposal_translations/actions/workflows/publish-proposal.yaml)

This repository contains the proposal for "Consistent Translations Glossary across R". The proposal aims to improve the technical infrastructure of the translations process across R projects. There are many volunteer translation efforts across the R community (messages in base R/recommended packages, rOpenSci materials such as their package development guide, Bioconductor training materials, R books such as R for Data Science, etc). These projects often have their own glossaries, since the benefits of using a glossary in translation projects are widely recognised (improves translation quality, reduces translation effort). However, developing and maintaining separate glossaries for each translation project reduces these benefits - different projects may use different translations for certain terms, effort to identify relevant terms and translate them is duplicated across projects putting unnecessary burden on volunteers. Some projects do not have the volunteer capacity to translate the glossary into multiple languages, or may not even use a glossary. Currently it is difficult for projects to take full advantage of existing glossaries due to diversity in the choice of translation infrastructure. These issues will become even more important if internationalization of R help pages becomes more common (ref R Consortium-funded project: [tooling-for-internationalization-of-r-help-pages](https://r-consortium.org/all-projects/2023-group-2.html#tooling-for-internationalization-of-r-help-pages))

An example of diverging translation of glossary terms is provided by the rOpensci English-Spanish glossary:

| English | Spanish (rOpenSci) | Spanish (R project)                        |
|--------|--------------------|--------------------------------------------|
| path    | ruta de acceso     | ruta (file path) / trayecto (polygon path) |   

that could be due to the term arising in different contexts though. There are many examples of diverging translations that might have been avoided if a glossary had been used, e.g. in base R "loop" is variously translated as "bucle", "loop", "ciclo" - both rOpensci and R project glossaries agree on "bucle" being the preferred term; sometimes "camino" is used rather than "ruta" for a file path. These don't change the meaning but may read a bit strangely. Since, there are limited glossaries to compare, it is difficult to provide more examples.

This proposal aims to address this issue by creating a data package in R package that will help maintain a consistent glossary to improve the quality of translations. This will help in making R more accessible to users who do not speak English and improve the overall user experience of R. Previously this problem has been discussed within the R Contribution Working Group (RCWG).

Feedback on the proposal is welcome - please feel free to provide your feedback by opening an issue in this repository.

## License

