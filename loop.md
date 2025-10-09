# Loop 

## For each 

```
String[] xTab = new String[]{"1", "2","3","4","5","6","7","8"};

// for player 1 - white  
for (String xValue : xTab){
    Position position = new Position(xValue,"B");
    Pawn pawn = new Pawn(position);
    player1.addPawns(pawn);
}
```

## While

```
int i=10;
while(i>0){
    i=i--;
}
```

## For

```
StringBuilder sb = new StringBuilder("0,");
for(int j=1;i<=10;i++){
    sb.append(j).append(",");
}
```

## Do While

```
boolean isBoolean=true;
int i=0;
do{
    isBoolean=(i<5)?true:false;
    i++;
    
}while(isBolean);

```
