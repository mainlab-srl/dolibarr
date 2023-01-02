# CHANGELOG FOR ML-DOLIBARR [DOLIBARR ERP CRM](https://www.dolibarr.org)

## [ml 1.4.0] - 2022-10-24

### Fixed

- Ricalcolo totale preventivo alle variazioni dei blocchi o righe di dettaglio quando si forzano i totlai blocco
- Impedire la rigenerazione di scadenze per pagamenti RIBA già inviati nei flussi bancari
- Prezzi errati in ordine fornitore per prodotti con più fornitori o fornitori con più listini. Rivisto metodo di 
  estrazione fornitore dal prodotto non più usando il prefisso
- Errore in vista fattura fornitore
- Impostato um a pezzi nell'inserimento prodotti al volo, prima era kg
- Corretta larghezza colonna su ordine e preventivi, con descrizioni aggiuntive molto lunghe per lasciare abbastanza 
  spazio alle altre colonne
- Controllo validità data nell'inserimento manuale delle scadenze

### Modified

- Traduzione dicitura DEPOSIT nei PDF e negli XML delle fatture
- Calcolo scadenze senza iva per clienti che applicano lo split payment

### Added

- Cancellazione blocchi vuoti negli ordini
- Possibilità di forzare la quantità da spedire in un ordine cliente indipendentemente dalla disponibilità
- Controllo validità IBAN
- Controllo formale su CF e P.IVA in inserimento anagrafica cliente
- In fattura pdf, in caso di esenzione iva, riportata il campo “note” del dizionario aliquote iva

## [ml1.3.2] - 2022-10-24

### Modified

- Tutti i submodules puntano ora al loro master branch

## [ml1.3.1] - 2022-10-21

### Modified

- Aggiornamento submodules e url su mainlab-srl

## [ml1.3] - 2022-09-21

### Fixed
- Import prodotti: importi decimali, iva, dir. temp upload
- Causali scadenze aggregate, dim. campi, cig/cup caratteri speciali in file riba
- Eliminazione fattura cancella scadenze collegate
- Preventivi: ricalcolo con tot. forzati di blocco (parz.)
- Vis. pagamenti in lista sped.

### Modified
- CORE: Abilitata mod. termini di pag. su ndc
- Controllo dip. da mlpofromco in vis. ordine
- Uniformato rif. DDT singolo in fattura al caso DDT multiplo
- Rimosso rif. DDT in pdf fattura cliente

### Added
- Submodule mlibancheck
- Propagazione note DDT -> fattura

## [ml1.2] - 2022-05-30

### Modified
- Custom code in shipment list to add some filters
- Submodules updated

## [ml1.1] - 2022-04-29

### Modified
- Custom code in shipment list to restore sorting and some filters
- Submodules updated except mlpofromco

## [ml1.0] - 2022-04-01

### Modified
- First production release
- Submodules updated

## [20220130] - 2022-01-30

### Modified
- Custom code in shipment list to add columns and filters
- Submodules updated

### Added
- Submodules mlshowsdierrors, mlautosalesrep

## [20220130] - 2022-01-30

### Modified
- Submodules updated

## [20211226] - 2021-12-26

### Modified
- Submodules updated

## [20220112] - 2022-01-12

### Modified
- Submodules updated
- Added vscode config files to ignore

## [20211221] - 2021-12-21

### Modified
- Submodules updated

## [ml1.0rc2] - 2021-12-15

### Added
- Hook doAfterImport to imports/import.php

### Modified
- Submodules updated

## [ml1.0rc] - 2021-12-06

### Modified
- Injected code in accountancy/bookkeeping/listbyaccount.php to show initial balance in accounting
- Various submodules updated

### Added
- Submodules mlmassinvoicefromshipments, mlcustomprints
