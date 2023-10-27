# Database Storage Strategy

### Decision

- We will implement **Encrypted Local Storage** for data persistence in the app.

### Rationale

- Local storage ensures that the app can function seamlessly without an active internet connection.
- Encrypting the local storage ensures that sensitive financial data remains secure, even if the device is compromised.

### Context

- Date: October 24, 2023
- Considering the sensitivity of financial data, it's imperative to prioritize data security. While cloud storage offers backup and multi-device sync advantages, the decision to exclude remote storage makes encrypted local storage the prime choice.
- Libraries such as `react-native-sensitive-info` can assist in securely storing data on the device.

### Consequences

- Users will have to ensure data backup manually, as there's no automatic cloud backup.
- Device loss or malfunction may result in data loss for the user.
- While encrypted local storage offers robust security, it's crucial to keep the encryption libraries up to date to prevent potential vulnerabilities.
