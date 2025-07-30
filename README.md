# 🎭 Playwright Test Suite

This project uses [Playwright](https://playwright.dev/) to perform end-to-end testing across modern browsers.

---

## 📦 ინსტალაცია

ტესტების გაშვებამდე აუცილებელია საჭირო პაკეტების დაყენება:

```bash
npm install
npx playwright install
npx playwright test
```

---

## ⚙️ ბრძანებების სია და მათი აღწერა

| ბრძანება | აღწერა |
|----------|--------|
| `npx playwright test` | ყველა end-to-end ტესტის გაშვება. |
| `npx playwright test --ui` | ინტერაქტიული UI რეჟიმის გაშვება ტესტირების მართვისა და დებაგინგისთვის. |
| `npx playwright test --project=chromium` | ტესტების გაშვება მხოლოდ Chromium ბრაუზერზე (მაგალითად, Google Chrome). |
| `npx playwright test example` | კონკრეტული ფაილის (მაგ. `example.spec.ts`) ტესტის გაშვება. |
| `npx playwright test --debug` | ტესტების გაშვება დებაგის რეჟიმში, Playwright Inspector-ის საშუალებით. |
| `npx playwright codegen` | ტესტების ავტომატური გენერაცია ბრაუზერში მოქმედებების ჩანაწერის საფუძველზე. |

---

## 📚 დოკუმენტაცია

- [📘 Playwright ოფიციალური დოკუმენტაცია](https://playwright.dev/)
- [🧪 ტესტების დამუშავება Playwright-ში](https://playwright.dev/docs/writing-tests)
- [⚙️ კონფიგურაციის სახელმძღვანელო](https://playwright.dev/docs/test-configuration)
- [💻 CLI ინსტრუქცია](https://playwright.dev/docs/test-cli)

---

## 📁 პროექტის სტრუქტურა

ტესტების სტანდარტული სტრუქტურა:

```
your-project/
├── tests/
│   ├── login.spec.ts
│   ├── homepage.spec.ts
├── pages/
│   │── BasePage.ts           # საერთო ქმედებები (base actions)
│   ├── LoginPage.ts              # LoginPage: იყენებს სელექტორებს და ფუნქციებს
│   └── HomePage.ts               # სხვა გვერდების Page ფაილები
│── selectors/
│   │── LoginSelectors.ts     # მხოლოდ სელექტორები
│   │── HomeSelectors.ts
├── utils/
│   └── test-fixtures.ts
├── playwright.config.ts
├── package.json
└── README.md

```

---

**წარმატებულ ტესტირებას გისურვებთ!** 🚀
