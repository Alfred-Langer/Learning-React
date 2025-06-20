# Understanding Server-Side Rendering in Older Websites

Older websites often used a technique called **Server-Side Rendering (SSR)**. With this technique the Server hosting the website would wait for a Client to request a specific webpage. Once the request was received, the Server would begin generating the corresponding HTML document.

This Server-side rendering process could involve various operations, such as performing calculations, querying a database, or calling an external API to gather necessary data. After retrieving and preparing the data, the Server would dynamically construct the HTML content, embedding the relevant information directly into the page.

Once the HTML document was fully rendered, it would be sent back to the Client's browser. The HTML would typically include references to external CSS and JavaScript files, which the browser would then load separately.

On the Client side, JavaScript was usually minimal and handled small tasks such as animations or form validation. The majority of dynamic content—such as displaying a list of YouTube videos or updating a stock price chart—was processed and rendered on the Server before being delivered to the browser.

This approach ensured that users received a fully-formed page quickly and reliably, even with minimal Client-side scripting.



# Understanding how Modern Web Applications are rendered

It's more common nowadays for websites to use a design pattern known as SPA or "Single Page Application". The idea
behind this is that the Client will make a request to the Server, and the Server will respond with a very minimal HTML document and a bundle of JavaScript. This bundle of Javascript would be the actual modern web application built with ReactJS, Vue, or Angular. When this JavaScript bundle is executed on the Client's browser, it will dynamically update the DOM and render the web page. This is what would be known as Client-Side Rendering. This way, any external data-retrieval like contacting a Database or an External API can be done so on the Client's browser instead of taxing the Server. 


# Understanding How Modern Web Applications Are Rendered

Modern websites often use a design pattern known as a **Single Page Application (SPA)**. In this approach, the client (typically a web browser) makes an initial request to the server, which responds with a minimal HTML document and a bundled JavaScript file.

This JavaScript bundle contains the actual web application, usually built using modern frameworks such as **React**, **Vue**, or **Angular**. When the browser downloads and executes this bundle, it dynamically updates the DOM and renders the user interface directly in the browser. This rendering strategy is known as **Client-Side Rendering (CSR)**.

Instead of fetching and rendering a new HTML page with each interaction, SPAs rely on client-side routing to update the visible content. Any necessary data, such as user information or live updates, is typically fetched via APIs (e.g., REST or GraphQL) and inserted into the DOM dynamically. This allows for a more seamless user experience and can reduce the load on the server by offloading UI rendering to the client.

While much of the UI logic resides in the browser, the server still plays a key role in handling data storage, authentication, and secure business logic.
