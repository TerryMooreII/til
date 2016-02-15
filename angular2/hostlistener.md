# HostListener() Annotations

Angular will invoke the decorated method when the host element emits the specified event.

```typescript
@Directive({selector: 'button[counting]'})
class CountClicks {
  numberOfClicks = 0;
  @HostListener('click', ['$event.target'])
  onClick(btn) {
    console.log("button", btn, "number of clicks:", this.numberOfClicks++);
  }
}
@Component({
  selector: 'app',
  template: `<button counting>Increment</button>`,
  directives: [CountClicks]
})
class App {}
bootstrap(App);
```

[Source](https://angular.io/docs/js/latest/api/core/HostListener-var.html)
