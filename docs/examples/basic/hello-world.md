---
title: Hello World!
keywords:
 - javascript
 - tour
 - guide
---

import { LiveExample } from "../../../lib/liveExample.js";


You can create your product tour using `data-intro` and `data-title` HTML attributes. Simply add those attributs to your
elements and call `introjJs().start()`:

```jsx
<div data-title="Welcome!" data-intro="Hello World! 👋" class="card-demo">
  <div class="card shadow--md">
    <div class="card__image" data-intro="Intro.js can highlight on elements">
      <img
        src="..."
        alt="Image alt text"
        title="Logo Title Text 1"
      />
    </div>
    <div class="card__body" data-title="Farewell!" data-intro="And this is the last step!">
      <h4>Quaco Lighthouse</h4>
      <small>
        The Quaco Head Lighthouse is a well maintained lighthouse close to St.
        Martins. It is a short, beautiful walk to the lighthouse along the
        seashore.
      </small>
    </div>
  </div>
</div>
```

<LiveExample children={
`// Intro.js scans the webpage and finds all elements with \`data-intro\` attribute
introJs();
`
} />

<br/>

<div class="demo-container">
    <div data-title="Welcome!" data-intro="Hello World! 👋" class="card-demo" style={{width: '300px'}}>
      <div class="card shadow--md">
        <div class="card__image" data-intro="Intro.js can highlight on elements">
          <img
            src="https://images.unsplash.com/photo-1506624183912-c602f4a21ca7?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=800&amp;q=60"
            alt="Image alt text"
            title="Logo Title Text 1"
          />
        </div>
        <div class="card__body" data-title="Farewell!" data-intro="And this is the last step!">
          <h4>Quaco Lighthouse</h4>
          <small>
            The Quaco Head Lighthouse is a well maintained lighthouse close to St.
            Martins. It is a short, beautiful walk to the lighthouse along the
            seashore.
          </small>
        </div>
      </div>
    </div>
</div>


