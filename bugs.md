## Subscription stops

Can't reproduce.
When I'm clearing cache and everything

## Reactivity

You're trying to run method of parent's scope inside callback which is outside the digest cycle.

```javascript
// columnSort.directive.ts:67
wrapper.on( 'click', ( e ) => {
  this.doSort( e.currentTarget );
});
```
