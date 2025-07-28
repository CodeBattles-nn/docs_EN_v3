# Table of contents

* [About the V3 System](README.md)
* [Contribution Guidelines](contribution-guidelines.md)

## Overview

* [Participant Interface](obzor/interfeis-uchastnika.md)
* [Administrator Interface](obzor/interfeis-administratora/README.md)
  * [Tasks](obzor/interfeis-administratora/zadachi.md)
  * [Users](obzor/interfeis-administratora/polzovateli.md)
  * [Checkers](obzor/interfeis-administratora/chekery.md)
  * [Competitions](obzor/interfeis-administratora/sorevnovaniya.md)

## System Setup and Installation

* [Installation](nastroika-i-ustanovka-sistemy/ustanovka/README.md)
  * [Local Installation](nastroika-i-ustanovka-sistemy/ustanovka/lokalnaya-ustanovka.md)
  * [Production Installation](nastroika-i-ustanovka-sistemy/ustanovka/production-ustanovka.md)

## First Competition

* [Create a Competition](pervoe-sorevnovanie/sozdat-sorevnovanie.md)

## Instructions

* [Change Language](instrukcii/smena-yazyka.md)
* [Competition](instrukcii/sorevnovanie/README.md)
  * [Creating a Competition](instrukcii/sorevnovanie/sozdanie-sorevnovaniya.md)
  * [Editing Competition Checkers](instrukcii/sorevnovanie/redaktirovanie-chekerov-sorevnovaniya.md)
  * [Editing Competition Users](instrukcii/sorevnovanie/redaktirovanie-polzovatelei-sorevnovaniya.md)
  * [Editing Competition Tasks](instrukcii/sorevnovanie/redaktirovanie-zadach-sorevnovaniya.md)
* [Tasks](instrukcii/zadachi/README.md)
  * [Add a Task](instrukcii/zadachi/dobavit-zadachu.md)
  * [Modify a Task](instrukcii/zadachi/izmenit-zadachu.md)
  * [Delete a Task](instrukcii/zadachi/udalit-zadachu.md)
  * [Import from Polygon System](instrukcii/zadachi/import-iz-sistemy-polygon.md)
* [Users](instrukcii/polzovateli/README.md)
  * [User Registration](instrukcii/polzovateli/registraciya-polzovatelei.md)
* [Checkers](instrukcii/chekery/README.md)
  * [Creating a Checker](instrukcii/chekery/sozdanie-chekera.md)
  * [Modifying a Checker](instrukcii/chekery/izmenenie-chekera.md)
  * [Deleting a Checker](instrukcii/chekery/udalenie-chekera.md)

## How the System Works

* [Architecture](kak-rabotaet-sistema/arkhitektura.md)
* [Security](kak-rabotaet-sistema/bezopasnost.md)
* [Code Line Metrics](kak-rabotaet-sistema/metriki-strok-koda.md)

## API

* [Introduction to API](api/vvedenie-v-api.md)
* [Backend](api/backend/README.md)
  * ```yaml
    type: builtin:openapi
    props:
      models: true
    dependencies:
      spec:
        ref:
          kind: openapi
          spec: doctorixx-api
    ```
* [Checker API](api/checker-api/README.md)
  * ```yaml
    type: builtin:openapi
    props:
      models: false
    dependencies:
      spec:
        ref:
          kind: openapi
          spec: codebattles-checker-api
    ```