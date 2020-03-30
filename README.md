# 2020-social_distancing

**Live demos**
* http://plus.yle.fi/dev/2020-03-nrk_simulaatio/faster-simulation.html
* http://plus.yle.fi/dev/2020-03-nrk_simulaatio/slower-simulation.html

## Animation shows how the spread of COVID-19 can be restricted with social distancing (NRK)

Many countries are implementing restrictions to people's movement. The visualisation shows how social distancing affects the spread on the COVID-19.

**Original article (English and Norwegian version)**
* [Social distancing against Corona explained](https://www.nrk.no/norge/xl/social-distancing-against-corona-explained-1.14955285)
* [Slik virker den nasjonale koronadugnaden](https://www.nrk.no/norge/xl/slik-virker-den-nasjonale-koronadugnaden-1.14947139)

**Inspired by**
* [Why outbreaks like coronavirus spread exponentially, and how to “flatten the curve”](https://www.washingtonpost.com/graphics/2020/world/corona-simulator/)

**EBU links**
* [News Exchange](https://news-exchange.ebu.ch/item_detail/47d4c3872f549a6186f7e26edc71ab35/2020_21014527)

**Used by**
* [Yle/Finland on Online](https://yle.fi/uutiset/3-11272825)

## How to use

If you are interested in using the interactive version please contact Teemo Tebest, tebest@ebu.ch

This visualization is part of the EBU News Exchange’s Data Journalism project. Other projects are available: https://news-exchange.ebu.ch/data-journalism

## Rights of usage

Access only for EBU Members and Sub-Licensees participating in the News Exchange (for full list see: https://www.ebu.ch/eurovision-news/members-and-sublicensees). Coverage cannot be used by a national competitor of the contributing broadcaster on the national territory.

## How to build and develop

This is Yle/Finland's version of NRK/Norway's visualization. Original NRK implementation is included in `simulator.zip`.

YleApp is found from `/src/ts/components/YleApp`.

Modified NRK app is found from `src/ts/components/App`

There are two entrypoint for video capture `faster-simulation.html` and `slower-simulation.html`.

### Install dependencies

`yarn install`

### Start app

`yarn start`

### Linting:

`yarn lint-ts`

### Building

There are two different build commands for Yle enviroments: test and production.

`yarn build-dev`

`yarn build-prod`

If you want to use same build commands change ASSET_PATH to match your enviroment.

### Sync into production

AWS commands work only on Yle enviroment.

### Preview:

By default project runs in localhost port 3000.

Standalone dev:
`http://localhost:3000`
