
# 🧮 Calculator - Solidity Contract

This smart contract implements a basic **calculator in Solidity** that performs simple arithmetic operations, including addition, subtraction, and multiplication, supporting both unsigned (`uint256`) and signed (`int256`) integers.

---

## 📖 Description

- **Available operations:**
  - ➕ **Addition (`addition`)**
  - ➖ **Subtraction (`substraction`, `substraction2`)**
  - ✖️ **Multiplication (`multiplier`, `multiplier2`)**
- **Events:** `Addition` and `Substraction`.
- **Modifiers:** `checkNumber` (restricts execution if the argument is not `10`).
- **State variable:** `resultado` (initialized to `10`).

---

## ⚙️ Requirements

- **Solidity version:** `0.8.24`
- Compatible with **0.8.x and above**.

---

## 🚀 Usage

1. **Deploy the contract** on any EVM-compatible network.
2. **Main functions:**
   - `addition(uint256 num1_, uint256 num2_)`: Adds two numbers and emits `Addition`.
   - `substraction(uint256 num1_, uint256 num2_)`: Subtracts two unsigned numbers and emits `Substraction`.
   - `substraction2(int256 num1_, int256 num2_)`: Subtracts two signed numbers.
   - `multiplier(uint256 num1_)`: Multiplies `resultado` by `num1_`.
   - `multiplier2(uint256 num1_)`: Same as `multiplier`, but only if `num1_ == 10`.

---

## 📡 Events

- **Addition:** Logs added values and the result.
- **Substraction:** Logs subtracted values and the result.

---

## 🔒 Security Considerations

- Subtraction with `uint256` may cause *underflow* if `num2_ > num1_`.
- `checkNumber` prevents unwanted multiplications in `multiplier2`.
- No access control (*onlyOwner*) is implemented.

---

## 📜 License

This project is licensed under **LGPL-3.0-only**.


# 🧮 Calculadora - Contrato en Solidity

Este contrato inteligente implementa una calculadora básica en **Solidity** que permite realizar operaciones aritméticas simples, incluyendo suma, resta y multiplicación, con soporte para enteros sin signo (`uint256`) y con signo (`int256`).

---

## 📖 Descripción

- **Operaciones disponibles:**
  - ➕ **Suma (`addition`)**
  - ➖ **Resta (`substraction`, `substraction2`)**
  - ✖️ **Multiplicación (`multiplier`, `multiplier2`)**
- **Eventos:** `Addition` y `Substraction`.
- **Modificadores:** `checkNumber` (restringe ejecución si el argumento no es `10`).
- **Variable de estado:** `resultado` (inicializado en `10`).

---

## ⚙️ Requisitos

- **Versión de Solidity:** `0.8.24`
- Compatible con compiladores **0.8.x y superiores**.

---

## 🚀 Uso

1. **Despliega el contrato** en una red compatible con la EVM.
2. **Funciones principales:**
   - `addition(uint256 num1_, uint256 num2_)`: Suma dos números y emite `Addition`.
   - `substraction(uint256 num1_, uint256 num2_)`: Resta dos números sin signo y emite `Substraction`.
   - `substraction2(int256 num1_, int256 num2_)`: Resta dos números con signo.
   - `multiplier(uint256 num1_)`: Multiplica `resultado` por `num1_`.
   - `multiplier2(uint256 num1_)`: Igual que `multiplier`, pero solo si `num1_ == 10`.

---

## 📡 Eventos

- **Addition:** Registra los valores sumados y el resultado.
- **Substraction:** Registra los valores restados y el resultado.

---

## 🔒 Consideraciones de seguridad

- La resta con `uint256` puede provocar *underflow* si `num2_ > num1_`.
- `checkNumber` evita multiplicaciones no deseadas en `multiplier2`.
- No incluye control de acceso (*onlyOwner*).

---

## 📜 Licencia

Este proyecto está licenciado bajo la **LGPL-3.0-only**.

---
