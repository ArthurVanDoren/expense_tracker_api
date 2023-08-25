Ik heb voor het project van API development gekozen om een "expense tracker" te maken.
Hier kan ik dus een gebruiker registreren en vervolgens een item toevoegen waar ik een beschrijving bij kan zetten. Zo kan ik het item de naam geven van de uitgave en dan bij description beschrijven hoeveel het gekost heeft.

Verder heb ik ook nog een webpagina gemaakt, dit is makkelijk om te gebruiken. Eerst maak je een gebruiker aan en dan kan er een item aan toevoegen. Die komen er dan vanonder op de pagina op te staan. Ook nog een simpele css layout is toegevoegd.

link naar de index.html: https://regal-sherbet-63b834.netlify.app/

## end points:

### app.get:
- @app.get("/") hiermee kan ik de webpagina bekijken
- @app.get("/users/", response_model=list[schemas.User]) dit lijst al de users op en dan nog data van de users
- @app.get("/users/{user_id}", response_model=schemas.User) hiermee kan ik de data van een users bekijken adhv de user id
- @app.get("/items/", response_model=list[schemas.Item]) hiermee kan ik al de items bekijken

### app.post:
- @app.post("/users/", response_model=schemas.User) zo kan ik een nieuw user aanmaken
- @app.post("/users/{user_id}/items/", response_model=schemas.Item) zo kan ik een nieuw item aanmaken

### app.delete:
- @app.delete("/items/{item_id}") zo verwijder ik een item 

### app.put:
- @app.put("/users/{user_id}", response_model=schemas.User) zo pas ik een user aan


## Screenshots:

![04](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/aa7c1b59-9fec-42f1-bc95-d43c0db2e9dd)
![03](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/bffeb12d-37e7-4a5b-b5a2-0bc7fbf8591c)
![02](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/4e803405-3de0-4f4d-b5d2-25b14e37db97)
![01](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/837ca5b9-ab52-4cb8-ad29-8c690f0f08c2)

## api docs:
![14](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/74f515bc-8709-4a54-95ef-266bc60fe476)
![06](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/06d2f855-3390-4634-8e2f-e44de6ad1437)
![07](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/8e27c026-6ffc-46bb-9bf6-f3df618fe320)
![08](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/79fa5bea-20df-4bf6-b09e-b713dbb407cf)
![09](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/d37892e8-0687-4e91-8634-00a9e7a9e351)
![10](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/9e045f42-9a1c-4fb3-9825-f910ff5c171c)
![11](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/a1e24722-79cb-409c-863f-58122c2c91fa)
![12](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/500f8c1a-7545-43b3-8ecf-1a53d33f7513)
![13](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/72b9fd6b-8b0e-4ad8-95c1-76e682810265)
![15](https://github.com/ArthurVanDoren/expense_tracker_api/assets/91262433/ca64bf81-b721-4e30-afa5-eaefd8b99722)
