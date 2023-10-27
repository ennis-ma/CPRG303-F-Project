# Choosing Development Framework and Styling Approach

### Decision

- We will develop the app using the **React Native** framework and utilize **CSS** for styling.

### Rationale

- **React Native** allows us to write most of our application's code once and run it on both Android and potentially iOS, leading to faster development and easier maintenance.
- React Native has a large community, which means extensive libraries, plugins, and community support.
- Using CSS for styling in React Native (via libraries like styled-components or React Native's built-in StyleSheet) ensures that developers with web development experience can easily adapt and contribute.

### Context

- Date: October 24, 2023
- Our target device platform is Android. However, by using React Native, there's potential flexibility to expand to other platforms in the future.
- CSS, being a widely adopted styling solution, ensures that our team can leverage existing knowledge and resources without the need for extensive retraining or adaptation.

### Consequences

- React Native might not always expose or fully support the very latest platform-specific features immediately upon their release.
- Some very platform-specific optimizations might not be achievable, potentially affecting performance or user experience.
- CSS, while familiar to many developers, will need to be used with React Native specifics in mind (for example, using flexbox for layout).
