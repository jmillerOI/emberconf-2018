
# Deep Dive on Ember Events

### Distinguish between DOM event listeners and Ember Event listeners
- DOM event listener (notice on* event syntax): <div onclick={{action 'handleClick'}}>click me</div>
- Ember event listener: <div {{action 'handleClick'}}>click me</div>
 - Ember event listeners don't receive the native DOM event
- DOM event listener fire before EMber event listeners
 
[Deep Dive on Ember Events Blog](https://medium.com/square-corner-blog/deep-dive-on-ember-events-cf684fd3b808)



[Video](https://youtu.be/bt9MRkf5Mus?t=14450)

[Slides](https://drive.google.com/file/d/1tI4_GJesVIiH1QXsHtjyT6NAyt0kip47/view)
