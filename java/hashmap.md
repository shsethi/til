1. Java documentation says

>If many mappings are to be stored in a HashMap instance, creating it with a sufficiently large capacity will allow the mappings to be stored more efficiently than letting it perform automatic rehashing as needed to grow the table.


2. Declarative way of adding values to map. 
```java
        Map<Integer,String> m = new HashMap<>();
        m.putIfAbsent(5,"1");
        m.putIfAbsent(5,"2");

        System.out.println(m.get(5)); //1

        System.out.println(m.computeIfAbsent(6, (k)->{
        return  "value for "+k;
        })); //value for 6
```
3. LetterCount or WordCount

```java

        Map<Character,Integer> wc = new HashMap<>();
        List<Character> l = Arrays.asList('a','b','c','d','e','a');

        l.forEach(letter->{
            wc.compute(letter,(k,v)->{
                if(v!=null) 
                    return v+1;
                else
                    return 1;
            });
        });

        System.out.println(wc); //{a=2, b=1, c=1, d=1, e=1}
```

Ref: https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html