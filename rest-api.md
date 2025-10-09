# Spring boot - Rest API

## Principles 

### RestController
Create a simple webservice 

First of all, create a class with annotation @RestController
inside define some methods permitting 
- @PostMapping
- @GetMapping
- @PutMapping
- @DeleteMapping

Each method (depending of what you want) is implementing a service.

```
@RestController("/v1/management") 
public class ProcessFileController{
    
    @PostMapping(name = "/file")
    pubic void postFile(){
    ....
    }

    @GetMapping(name = "/files")
    pubic void getFiles(){
    ....
    }

    @GetMapping(name = "/files/{id}")
    pubic File getFiles(@PathParam int id){
    ....
    }

}
```


### Service

A service annotation (@Service) is implementing a business logic and can call also another serviers. 
It depends of the context. 

```
@Service
public class Party {
    private Player player1 
    private Player player2
    
    @Autowired 
    public party(Player player1, Player player2){
        this.player1=player1;
        this.player2=player2;
    }
```

### Repository (JpaRepository)

Interface

```
@Repository
public Interface IPlayerRepository extends JpaRespository(Player,Long){

}

```

### Entity (table)

Table


```
@Entity
@Table(name = "PLAYER_DB")
public class Player{
    
    @ID
    @GenerateValue
    private Long ID;

    @Column(name = 'PLAYER_NAME')
    private String playerName;

}