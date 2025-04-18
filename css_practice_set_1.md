Perfect! Let's build **Tic-Tac-Toe** and **Chessboard** using only **`<div>`**, **`<table>`**, and **basic CSS properties** like `margin`, `padding`, `border`, `width`, `height`, `background-color` — no Flexbox or Grid.

---

## 🎯 Tic-Tac-Toe using `<div>` only

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .tictactoe {
      width: 312px;
      margin: 50px auto;
    }

    .row {
      height: 100px;
    }

    .cell {
      width: 100px;
      height: 100px;
      float: left;
      border: 2px solid black;
      text-align: center;
      line-height: 100px;
      font-size: 40px;
      background-color: #f5f5f5;
    }

    .clear {
      /* clear: both; */
    }
  </style>
</head>
<body>
  <div class="tictactoe">
    <div class="row">
      <div class="cell">X</div>
      <div class="cell">O</div>
      <div class="cell">X</div>
    </div>
    <div class="clear"></div>
    <div class="row">
      <div class="cell">O</div>
      <div class="cell">X</div>
      <div class="cell">O</div>
    </div>
    <div class="clear"></div>
    <div class="row">
      <div class="cell">X</div>
      <div class="cell">X</div>
      <div class="cell">O</div>
    </div>
    <div class="clear"></div>
  </div>
</body>
</html>
```

---

## ♟️ Chessboard using `<table>`

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    table.chess {
      border-collapse: collapse;
      margin: 50px auto;
    }

    td {
      width: 50px;
      height: 50px;
      border: 1px solid black;
    }

    .white {
      background-color: #ffffff;
    }

    .black {
      background-color: #000000;
    }
  </style>
</head>
<body>
  <table class="chess">
    <!-- 8 rows -->
    <!-- Alternate row starting color -->
    <tr>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
    </tr>
    <tr>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
    </tr>
    <tr>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
    </tr>
    <tr>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
    </tr>
    <tr>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
    </tr>
    <tr>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
    </tr>
    <tr>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
      <td class="white"></td><td class="black"></td><td class="white"></td><td class="black"></td>
    </tr>
    <tr>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
      <td class="black"></td><td class="white"></td><td class="black"></td><td class="white"></td>
    </tr>
  </table>
</body>
</html>
```

---

### ✅ Concepts Practiced:
- Box layout using `width`, `height`, `margin`, `padding`, and `float`
- Visual separation using `border`
- Coloring using `background-color`
- Table styling with alternating classes

---

Would you like to also:
- Add labels (like A–H, 1–8) to the chessboard?
- Create a game-like interaction for Tic Tac Toe with only CSS and checkboxes?

Let me know — happy to build it with you!


![alt text](image.png)