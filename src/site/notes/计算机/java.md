---
dg-publish: true
dg-hide: true
dg-hide-in-graph: true
---
#java

是否包含某个对象：
```java
public static void main(String[] args) {  
  int id = 2;  
  Integer[] showBottomNav = {2, 3, 4};  
  //List.of(showBottomNav).contains(id)  
  if (Arrays.stream(showBottomNav).anyMatch(i -> i == id)) {  
    System.out.println("contains");  
  } else {  
    System.out.println("not contains");  
  }  
}
```