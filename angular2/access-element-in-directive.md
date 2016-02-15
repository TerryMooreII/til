
# ElementRef 

Import `ElementRef` from `angular2/core`.  The reference it in your constructor like so.

```typescript
import { ElementRef, Directive} from 'angular2/core';

@Directive({
    selector: 'textarea'
})

export class Autosize {
  constructor(public element: ElementRef){
  }
  ngOnInit(){
      this.element.nativeElement.style.overflow = 'hidden';
  }
}
```
