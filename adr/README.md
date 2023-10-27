# Expense Tracker App: Architecture Decision Records (ADRs)

This repository contains the architecture decision records (ADRs) for the development of the Expense Tracker App. The application serves as a tool for users to manage and track their financial transactions, set budget goals, and visualize spending patterns.

## Overview

The Expense Tracker App is designed to offer a straightforward and user-friendly experience to maintain a clear record of both incomes and expenses. By providing visual aids and historical data, users can gain insights into their spending habits and make informed financial decisions.

## Decision Records:

1. [**App Framework and Platform**](framework-selection.md)
    - **Decision**: Hybrid application development using the React Native framework for Android devices.
    - **Rationale**: React Native enables efficient cross-platform development with a single codebase, allowing for quick market delivery and reduced maintenance efforts.
    - **Consequences**: While providing broader reach and reduced development time, the app might not utilize platform-specific optimizations to the fullest. A performance review will be scheduled post-development.

2. [**UI Toolkit**](ui-toolkit.md)
    - **Decision**: React Native Elements as the primary UI toolkit.
    - **Rationale**: This toolkit offers a comprehensive set of components that align with modern design principles, ensuring an appealing and consistent user experience. Its adaptability and community support further augment the development process.
    - **Consequences**: The team needs to familiarize themselves with React Native Elements if they haven't worked with it previously. However, the learning curve is relatively gentle.

3. [**Hardware Integration**](hardware-integration-for-security.md)
    - **Decision**: Integration with the device's Fingerprint scanner for enhanced security measures.
    - **Rationale**: As a financial tracking tool, the app handles sensitive information. Leveraging biometric authentication ensures a higher level of security, offering users confidence in the app's protective measures.
    - **Consequences**: Some users might not have devices equipped with fingerprint scanners. For them, alternative authentication methods will need to be in place.

4. [**Database Storage**](database-storage.md)
    - **Decision**: Local encrypted storage.
    - **Rationale**: Storing transaction data locally ensures quick access and reduced latency. Encryption is paramount to protect users' sensitive financial information.
    - **Consequences**: Local storage might have limitations on data volume. Regular data backup solutions and potential cloud syncing options should be considered for future releases.

The ADRs contained herein serve as a guideline and documentation for both current and future team members, ensuring a cohesive development journey and an understanding of the app's foundational decisions.

