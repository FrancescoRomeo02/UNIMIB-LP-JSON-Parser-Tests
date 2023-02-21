# UNIMIB-LP-JSON-Parser-Tests
Un tool per testare il corretto funzionamento del progetto JSONParser - Febbraio 2023


### How to
- Inserite il file `test.pl` nella stessa cartella dove avrete il file `jsonparse.pl`.
- Avviate l'ambiente Prolog e al posto di caricare il file "jsonparse", caricare il file "test". Si occuperà lui di caricare il vostro progetto.
- Avviate il predicato `test_all.`
- Questo eseguirà tutti i test presenti nel PDF della consegna per voi 😉

### Nota Bene
Ho notato che l'interprete Prolog nel caso debba printare a schermo un oggetto con tanti livelli di innestazione tende ad abbreviare un po' di cose con "| ..." (magari lo fa solo a me lol). Per ovviare a questa cosa è possibile utilizzare il seguente predicato:
```prolog
set_prolog_flag(answer_write_options,
    [ quoted(true),
        portray(true),
        spacing(next_argument)
    ]
).
```

Il test tiene conto degli oggetti **non abbreviati**. Per questo motivo potrebbe non darvi giusto alcuni casi. 

![proof-of-work](https://user-images.githubusercontent.com/86363063/220473031-618832bc-db81-401b-ba57-c4f6948a264e.gif)
