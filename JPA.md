### JPA


## One to One

```
@Entity
public class Student {
  @Id
  @GeneratedValue
  private Id Long;
  
  @OneToOne
  private Passport passport;
}

@Entity
public class Passport {
  ...
  
  @OneToOne(mappedBy="student) //if you want bi-directional
  
}
```
