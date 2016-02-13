# Annotations

I found out the hard way while standing up a new Angular 2 project that Typescript annotation have a () at the end unlike Java Spring.

```javascript

@Injectable()
export class Name{ ... }

```

**not**

```java

@Service
public class Name { ... }

```
