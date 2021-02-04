<!-- Istruzioni:
Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato.
 -->

# database name: Store

# nome tabelle: Videogames

- id            BIGINT PRIMARYKEY NOTNULL AUTO_INCREMENT UNIQUE
- title         string VARCHAR (50) NOTNULL
- platform      string VARCHAR(25) NULL
- format        string VARCHAR(25) NULL
- genre         string VARCHAR(15) NOTNULL
- cover_image   string VARCHAR(250) NULL
- publisher     string VARCHAR(30) NOTNULL
- developer     string VARCHAR(50) NULL
- barcode       string VARCHAR(13) NOTNULL UNIQUE
- sku           string VARCHAR(20) NOTNULL UNIQUE
- pegi          number SMALLINT NULL
- language      string VARCHAR(20) NOTNULL
- price         number FLOAT(6,2) 9999,99 NULL
- availability  number TINYIT NULL DEFAULT(0)
- quantity      number SMALLINT NULL DEFAULT(0)
- description   string TEXT NULL
- topic         string VARCHAR(30) NOTNULL
- edition       string VARCHAR(20) NULL
- release_date  data DATE NOTNULL
- created       data DATETIME NOTNULL
- edited        data DATETIME NULL