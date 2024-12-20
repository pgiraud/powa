# PoWA V5 - Quoi de neuf ?

## Introduction

### PostgreSQL Workload Analyzer - kesako ?

### A quoi ça sert ?

### À qui ça sert ?

### Sondage

### Problèmes résolus

### Description (rapide) des composants

 - extensions:
   - pg_stat_statements
   - pg_stat_kcache
   - pg_qualstats
   - pg_wait_sampling
   - pg_track_settings
   - powa_archivist
 - powa-collector
 - powa-web

<!-- Schéma -->

## V5 - Refonte de l'interface

### But

Moderniser le code

### Historique

V1 & V2

<!-- captures -->

### Réécriture : Quand ?

Début du développement courant de l'été 2022, temps R&D Dalibo.

### Réécriture : libraries

Backbone.js
Foundation Framework
Rickshaw
Bower

->

VueJS
Vuetify
D3.js
ViteJS

### Réécriture : Découpage  

Fonctionnement initial conservé

Structure arborescente et widgets

Structure représentée dans un objet JSON,
Chaque widget est responsable de faire les requêtes pour obtenir ses données

### Réécriture : pseudo SPA

Quasi Single Page App

-> meilleure expérience utilisateur

<!-- vidéo comparative v4 & v5 -->

## Quelques fonctionnalités phares de PoWA

### "Optimiser base"

Suggestion d'indexes

## Autres nouveautés de la v5

UI :
- mode sombre / clair
- sélecteur de dates

Back end / Métriques :
- Add pg_stat_activity graphs on the per-server and per-db pages (Julien Rouhaud)
- Add table / index bar graphs on the per-server and per-db pages (Julien Rouhaud)
- Add pg_stat_archiver widgets (Julien Rouhaud)
- Add pg_stat_replication widgets (Julien Rouhaud)
- Add pg_stat_database widgets (Julien Rouhaud)
- Add pg_stat_replication_slots widgets (Julien Rouhaud)
- Add pg_stat_io widgets (Julien Rouhaud)
- Add pg_stat_database_conflicts widgets (Julien Rouhaud)
- Add pg_stat_slru widgets (Julien Rouhaud)
- Add pg_stat_wal widgets (Julien Rouhaud)
- Add pg_stat_wal_receiver widgets (Julien Rouhaud)
- Add pg_stat_subscription(_statistic) widgets (Julien Rouhaud)
- Handle new IO timing and JIT counters added in newer pg_stat_statements versions (Julien Rouhaud)
<!-- FIXME à compléter -->

Support de PG17

## Idées d'améliorations / futur

- Davantage de messages explicatifs pour guider les utilisateurs
- Enregistrement d'instances via l'interface web
