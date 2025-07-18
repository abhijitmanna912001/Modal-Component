# 🧩 React Modal – Compound Component Design Pattern

This project showcases a reusable **Modal component** built using the **Compound Component Design Pattern** in React with TypeScript.

🔗 **Live Demo**: [extraordinary-dragon-ffa56f.netlify.app](https://extraordinary-dragon-ffa56f.netlify.app/)

---

## ✨ Features

- Composable modal structure using nested subcomponents
- Modal visibility controlled using `useState`
- Customizable `Title`, `Body`, and `Footer` sections
- Clean, centered UI with a backdrop overlay
- Fully responsive and accessible structure

---

## 🧱 Compound Component Structure

The `Modal` component exposes three subcomponents via static properties:

```tsx
Modal.Title = ModalTitle;
Modal.Body = ModalBody;
Modal.Footer = ModalFooter;
```

This structure allows developers to compose the modal in a declarative, flexible way:

```tsx
<Modal>
  <Modal.Title>...</Modal.Title>
  <Modal.Body>...</Modal.Body>
  <Modal.Footer>...</Modal.Footer>
</Modal>
```

Each subcomponent handles its respective section within the modal, making the layout easy to customize while keeping the parent `Modal` component clean.

---

## 🛠️ How It Works

- The `Modal` component renders a centered white box over a dark overlay.
- `Modal.Title`, `Modal.Body`, and `Modal.Footer` are imported separately and assigned as static properties to the main `Modal` component.
- The parent component (`App`) uses `useState` to toggle the modal open or closed.
- Modal content is passed as `children` to allow maximum flexibility.

---

## 📦 Tech Stack

- **React** (with TypeScript)
- **Tailwind CSS** (or regular CSS)
- **Vite** or Create React App

---

## 🚀 Getting Started

```bash
npm install
npm run dev
```

Use `useState` in your application to control modal visibility and compose the modal using the compound components pattern.

---

## 🧠 What You’ll Learn

- How to structure reusable and declarative components in React
- How to apply the **Compound Component Design Pattern**
- How to manage UI component visibility cleanly

---

## ✅ Possible Enhancements

- [ ] ESC key to close modal
- [ ] Click outside to dismiss
- [ ] Add open/close animations
- [ ] Improve accessibility (focus trap, ARIA labels)

---

This project is a solid foundation for building more advanced modals or even your own React component library!
