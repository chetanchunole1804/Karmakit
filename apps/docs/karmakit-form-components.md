
# 📦 Form Components Documentation (`karmakit/forms`)

## 🚀 Goal
To provide **well-styled**, **customizable**, and **reusable** input and form components with good defaults, which can be extended using `style` or `className` props.

---

## 📂 Component Categories

### 1. 🧩 Input Components (Styled React Components)

These are raw styled input fields that serve as building blocks for form creation:

| Component Name           | Description                             |
|--------------------------|-----------------------------------------|
| `Checkbox`               | Single checkbox input                   |
| `Checkboxes`             | Multi-select checkbox group             |
| `Color`                  | Color picker input                      |
| `Date`                   | Date input field                        |
| `DateTime`               | Date & time input combined              |
| `Email`                  | Email address input                     |
| `File`                   | File upload input                       |
| `FinancialWeek`          | Custom week selector (for finance)      |
| `Month`                  | Month picker input                      |
| `Number`                 | Numeric input field                     |
| `Password`               | Password input with toggle visibility   |
| `Range`                  | Slider input (min-max)                  |
| `Telephone`              | Telephone number input                  |
| `Text`                   | Standard text input                     |
| `Time`                   | Time picker input                       |
| `URL`                    | Website URL input                       |

---

### 2. 📥 Select & Button Components

| Component Name           | Description                             |
|--------------------------|-----------------------------------------|
| `Select`                 | Styled dropdown / select field          |
| `BusinessSearch`         | Searchable dropdown for businesses      |
| `SubmitButton`           | Styled form submit button               |

---

### 3. 🧾 Form Component Variants

These are higher-level components or ready-to-use templates built using the input components.

| Form Type              | Description                                   |
|------------------------|-----------------------------------------------|
| `BasicForm`            | Simple form layout with label, input, error   |
| `MultiStepForm`        | Step-based form flow                          |
| `WizardForm`           | Form with dynamic steps and validations       |
| `InlineForm`           | Compact form with inline fields               |
| `SearchForm`           | Form with search input and filters            |
| `DynamicForm`          | Form generated from JSON config or schema     |

---

## ✨ Customization

All components accept the following optional props for maximum flexibility:

- `style`: Inline CSS styles
- `className`: Override styles using your own CSS or Tailwind classes
- `variant`: Optional predefined styling variants (like `primary`, `flat`, `ghost`)
- `theme`: Coming soon (global theming support via context)

---

## 🔧 Usage Example

```tsx
import { Text, Email, Password, SubmitButton } from '@karmakit/forms';

export default function SignupForm() {
  return (
    <form className="flex flex-col gap-4">
      <Text label="Full Name" name="name" />
      <Email label="Email Address" name="email" />
      <Password label="Create Password" name="password" />
      <SubmitButton label="Sign Up" />
    </form>
  );
}
```

---

<!-- ## 📅 Work In Progress

> These components are currently being developed and will be released incrementally.

- ✅ Core input components
- 🚧 Complex form types
- 🧪 Schema-based dynamic form (future plan)
- 🎨 Theming & customization system

---

## 👨‍💻 Author

**Chetan Chunole**  
Full Stack Developer | Open Source Contributor  
[GitHub](https://github.com/yourgithub) • [LinkedIn](https://linkedin.com/in/yourprofile) -->
