# lazy-route - Lazy route loading for React Router 4 through System.import

#### Dependencies and requirements

This component only works with React Router 4 and Webpack 2 (because of System.import).

#### Usage

```javascript
import {Match} from 'react-router'
import LazyRoute from 'lazy-route'

<Match 
  pattern="/myroute"
  render={(props) => <LazyRoute {...props} component={System.import('./myComponent')} />}
/>
```

#### Upcoming features
The component works, but I have yet to add tests and some polish to it,
the plan is to add a customizable loader etc.
