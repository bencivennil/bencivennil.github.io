### Compressione
```
zip -rq <file> <directory>
tar cfSz <archivio.tar.gz> <directory_da_archiviare>
```

### Decompressione

```
unzip <file>
tar xfz <archivio.tar.gz>
```

### Copia il file locale sul server remoto

```
scp file.tgz user@server:
```

### Copia in locale il file sul server remoto
```
scp user@server:file.tgz .
```

## Ricerca
### Trova dalla directory corrente i file a 0 byte

```
find . -size 0
```
```
find . -name \*.php -exec grep -Hin "<stringa>" {} \;
```

```
grep -Hin '<stringa_da_cercare>' <cartella o gruppo di file * in cui cercare>
```

## MYSQL
### Backup

```
mysqldump -u root -p[root_password] [database_name] > dumpfilename.sql
```

### Restore

```
mysql -u root -p[root_password] [database_name] < dumpfilename.sql
```