# Sendexa Node.js SDK

Official Node.js SDK for the **Sendexa Communications Platform**.

Sendexa allows developers to integrate **SMS, OTP, Email, Voice, and USSD** into their applications through simple APIs.

---

## Installation

```bash
npm install sendexa
```

or

```bash
bun add sendexa
```

---

## Quick Start

```ts
import { Sendexa } from "sendexa";

const sendexa = new Sendexa({
  apiKey: process.env.SENDEXA_API_KEY
});

await sendexa.sms.send({
  to: "+233XXXXXXXXX",
  from: "SENDEXA",
  message: "Hello from Sendexa 🚀"
});
```

---

## Features

* SMS messaging
* OTP verification
* Email delivery
* Voice calls
* USSD sessions
* Developer-first API design

---

## Example

Send OTP:

```ts
await sendexa.otp.send({
  to: "+233XXXXXXXXX",
  channel: "sms"
});
```

Verify OTP:

```ts
await sendexa.otp.verify({
  to: "+233XXXXXXXXX",
  code: "123456"
});
```

---

## Documentation

Full documentation available at:

https://docs.sendexa.co

---

## Contributing

We welcome contributions from the community.

Please open an issue or submit a pull request.
