# 🍃 Leaf – Peer-to-Peer Car and Driver Rental

Leaf is a car rental marketplace prototype. Car owners earn money by renting out their cars for a day or more, customers rent them (with or without a driver), and Leaf acts as the mediator that splits the payment and keeps a commission.

> **Status:** working prototype. Payments are simulated and data is stored in the browser (localStorage). There is no login or backend yet.

## Features

- **Car owners** list a car with photo, brand, model, price per day and suitable terrains. An owner can also register as a driver for their own car.
- **Customers** filter cars by terrain, choose 1–7 days, optionally add a driver, and see a full price breakdown before paying.
- **Drivers** register the brands/variants and terrains they can drive and their rate per day. Only matching drivers are offered for a car.
- **Handover and inspection:** the driver (or customer, if self-drive) collects the car and keys from the owner and must tick a 5-point inspection checklist before taking the car.
- **Commission model:** Leaf keeps 10% from the owner's share and 10% from the driver's share. The Earnings screen shows all payouts.

## Screenshots

| Rent | Booking | List a car |
|---|---|---|
| ![Rent](screenshot-rent.png) | ![Booking](screenshot-booking.png) | ![List car](screenshot-list-car.png) |

| Driver registration | Inspection | Earnings |
|---|---|---|
| ![Driver](screenshot-driver.png) | ![Inspection](screenshot-inspection.png) | ![Earnings](screenshot-earnings.png) |

## How it works

1. Owner lists a car → 2. Customer books it (± driver) → 3. Driver goes to the owner and inspects the car → 4. Car delivered to the customer → 5. Car returned to the owner → 6. Payouts released minus commission.

## Run locally

No installation needed.

1. Download or clone this repository.
2. Open `index.html` in a browser, or open the folder in VS Code and use the **Live Server** extension (right-click `index.html` → *Open with Live Server*).

## Project structure

```
├── index.html
├── style.css
├── script.js
├── README.md
├── LICENSE
├── Leaf_Project_Report.docx
└── screenshot-*.png
```

## Configuration

- Commission rate: `COMM` at the top of `script.js` (default `0.10`).
- Brands, terrains and sample data: constants at the top of `script.js`.

## Tech stack

HTML5, CSS3, vanilla JavaScript (ES6), FileReader API, localStorage.

## Roadmap

- Flask + SQL backend and user login
- Real payment gateway and payouts
- Driving licence / ID / vehicle document verification
- Availability calendar to prevent overlapping bookings
- Insurance, damage claims, GPS tracking, ratings and reviews

## Author

**Adarsh Raj** – MCA (AI & ML), Chandigarh University (2025–2027)

## License

MIT – see [LICENSE](LICENSE).
