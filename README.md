# restaurants-mysql-ds
Generate Fake JSON documents for the restaurant collection using MySQL X Protocol


## Import JSON

Using MySQL Shell:

```
    JS > session.createSchema('docstore')
    <Schema:docstore>
    JS > \u docstore
    Default schema `docstore` accessible through db.
    JS > util.importJson('restaurants.json', {convertBsonOid: true})
    Importing from file "restaurants.json" to collection `docstore`.`restaurants`
     in MySQL Server at 10.0.1.249:33060
    
    .. 25359.. 25359
    Processed 15.60 MB in 25359 documents in 0.9856 sec (25.36K documents/s)
    Total successfully imported documents 25359 (25.36K documents/s)
```


