# fppcommerce

> ⚠️ **Archive Notice:** This project is archived and no longer actively maintained. The live storefront has been discontinued.

## What the Project Does

**fppcommerce** is a multi-platform e-commerce solution comprising a **Next.js website** and a **Flutter Android app**. Both clients query a single backend via the **Shopify Storefront GraphQL API** and delegate transactions directly to Shopify’s hosted checkout.

* **Unified Catalog:** Serves real-time product collections, category filters, and detail pages across platforms.
* **Shared State & Persistence:** Web cart handling and Flutter app state management via `Provider`, with local theme preferences persisted via `shared_preferences`.
* **Externalized Payments:** Redirects checkout flows directly to Shopify’s secure hosted checkout interface.

---

## Why the Project Is Useful

1. **Headless E-Commerce Architecture:** Demonstrates how to decouple presentation layers from an e-commerce backend by consuming a single GraphQL endpoint across both web and native mobile clients.
2. **Cross-Platform Parity:** Showcases synchronous UX and data state handling across distinct application environments (React/TypeScript and Flutter/Dart).
3. **Academic Reference:** Built for **BSCS3-2S: ITE 401 (Platform Technologies)** and **ITE 245 (Programming Languages)** to evaluate client-server platform integration.

---

## How Users Can Get Started

### Prerequisites

* Node.js 18+ and npm
* Flutter SDK & Android SDK
* Active Shopify store domain and Storefront API token

### 1. Web Setup (Next.js)

1. Clone the repository:
```bash
git clone https://github.com/fpaulpalis/fppcommerce.git
cd fppcommerce

```


2. Install dependencies (estimated time: 2 minutes):
```bash
npm install

```


3. Create `.env.local` in the project root:
```env
SHOPIFY_STORE_DOMAIN=your-store.myshopify.com
SHOPIFY_STOREFRONT_ACCESS_TOKEN=your_storefront_access_token

```


4. Run the development server (estimated time: 1 minute):
```bash
npm run dev

```


5. Navigate to `http://localhost:3000`.

### 2. Mobile Setup (Flutter)

1. Enter the mobile directory:
```bash
cd flutter_app

```


2. Fetch dependencies (estimated time: 1 minute):
```bash
flutter pub get

```


3. Set your Storefront credentials in `lib/config.dart`:
```dart
const String shopifyDomain = 'your-store.myshopify.com';
const String storefrontAccessToken = 'your_storefront_access_token';

```


4. Run on a connected device or emulator (estimated time: 2 minutes):
```bash
flutter run

```



---

## Where Users Can Get Help

* Open a ticket via [GitHub Issues](https://www.google.com/search?q=https://github.com/fpaulpalis/fppcommerce/issues) for code defects or environment bugs.
* Refer to [Shopify Storefront API Documentation](https://shopify.dev/docs/api/storefront) for GraphQL schema queries.
* Inspect [ACKNOWLEDGEMENTS.md](https://www.google.com/search?q=ACKNOWLEDGEMENTS.md) for dependencies and licensing specifics.

---

## Who Maintains and Contributes to the Project

* **Author & Maintainer:** Francis Paul Palis ([@fpaulpalis](https://www.google.com/search?q=https://github.com/fpaulpalis))
* **Status:** Inactive. Pull requests and issues are unmonitored.
