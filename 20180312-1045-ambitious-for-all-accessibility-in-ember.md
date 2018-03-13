# Ambitious for All: Accessibility in Ember
- Accessibility Spec `WAI-ARIA` **Web Accessibility Initiative**

WCAG 2.0
- A
- AA
  - Federal Level Reqs
- AAA 
  - Encompases A + AA

- ADA
- A11Y
- Ember A11Y Project (GitHub)

### Accessibility is Emotional
- Users
  - Our Users, who need to perform their tasks for their daily lives
  - Use service that may have forgotten to make a11y
  - Frustration
  - Possibility of Exclusion

- Developers
  - Issues with pms pushing dates without a11y
  - Team lead pushing shipping before readiness on a11y
  
### Accessibility is Hard
- Spec is complex at times
- Ember Challenges
  - Routing Transitions
    - Screen reader doesn't recognize that something new has been added (required addon)
  - Modals
    - Limit use of modals for ADA compliance
    - Track focus within the modal until `esc` or item is picked, should not be able to ghost behind
  - ARIA-* Support
    - Need defined ruleset
  - Click all the things (actions)
    - Clicks should be translated over to the ability to hit enter as well
    - No nested interactive elements
  - Password issues with AT
    - SR will return as (star) *
    
** Webstards are key**

### The "Easy" Wins
- Use semantic HTML5
- Link vs Button
  - Use a link if it's a route, use a button if it's an action
- Keyboard Navigation
  - "If you're mouse can do it, your keyboard should be able to as well"
  - Keyboard shortcuts in AT (Look up)
- Color Contrast
  - Included in current chrome
- Image Alt Text
  - Add when relavent
  - Must be blank when used in a presentation sense
  - When shopping or need to extend on the look or description of the image, use alt text

- Aria Level Rule
```
<div aria-level="1">Page Title</div>
```

```
<h1>Page Title</h1>
```

### There's an Addon for that
Ember-A11y
Ember-A11y-Testing
Ember-A11y-Landmarks
A11y-Announcer
Ember-Cli-Template-Lint

### Keep In Mind
- Keyboard Navigation
- Focus Navigation
- Aria-* Support
- Render Semantic HTML
- Image Alt Text

## Be Magnanimous
    
#### Keywords
AT - Assistive Technology
SR - Screen Reader


##### Speaker
Melanie Sumner
    
