# Java NetBeans Mini Projects (Apache NetBeans IDE 16)

This repository contains **three separate Java Swing GUI applications**, each packaged as its own **NetBeans/Ant project**:

- **CrossNKnot** – a simple **Tic‑Tac‑Toe (X/O)** game for two players.
- **siCalculator** – a **Simple Interest** + **Total Amount** calculator.
- **simpleScientificCalculator** – a **scientific calculator** (basic + scientific functions).

All projects were created with **Apache NetBeans IDE 16** and are configured for **Java 16** (`javac.source=16`, `javac.target=16`).

---

## Project structure

```
Project-of-Java-Apache-NetBeans-IDE16-master/
  CrossNKnot/
    src/crossnknot/...
  siCalculator/
    src/sicalculator/...
  simpleScientificCalculator/
    src/simplescientificcalculator/...
```

Each folder above is an independent NetBeans project with its own `build.xml`, `nbproject/`, and `src/`.

---

## Apps and main classes

| App | Folder | Main class |
|---|---|---|
| Tic‑Tac‑Toe (X/O) | `CrossNKnot/` | `crossnknot.XO_Game` |
| Simple Interest Calculator | `siCalculator/` | `sicalculator.simpleInterestCalc` |
| Scientific Calculator | `simpleScientificCalculator/` | `simplescientificcalculator.ScientificCalculator` |

---

## Requirements

- **JDK 16+** (or change the project `javac.source` / `javac.target` if you want to use an older/newer JDK).
- One of:
  - **Apache NetBeans IDE 16** (recommended), or
  - **Apache Ant** + a terminal (NetBeans projects use Ant under the hood)

---

## Run with Apache NetBeans (recommended)

1. Install **JDK 16+** and **Apache NetBeans IDE 16**.
2. Open NetBeans.
3. Go to **File → Open Project…**
4. Select **one** of these folders:
   - `CrossNKnot`
   - `siCalculator`
   - `simpleScientificCalculator`
5. Click **Run** (green ▶) to start the application.

> Each folder is a separate project — open/run them one at a time, or open all three as separate projects.

---

## Run from the command line (Ant)

From the repository root (or from inside any project folder), run:

### 1) CrossNKnot (Tic‑Tac‑Toe)
```bash
cd CrossNKnot
ant clean run
```

### 2) siCalculator (Simple Interest)
```bash
cd siCalculator
ant clean run
```

### 3) simpleScientificCalculator (Scientific Calculator)
```bash
cd simpleScientificCalculator
ant clean run
```

### Build JAR files
To build a runnable JAR for a project:

```bash
ant clean jar
```

The output will be created under the project’s `dist/` folder, for example:
- `CrossNKnot/dist/CrossNKnot.jar`
- `siCalculator/dist/siCalculator.jar`
- `simpleScientificCalculator/dist/simpleScientificCalculator.jar`

You can run a built JAR with:

```bash
java -jar dist/<jar-name>.jar
```

---

## How to use each app

### CrossNKnot (Tic‑Tac‑Toe)
- It is a **two‑player** game using **X** (Player 1) and **O** (Player 2).
- Players enter a **position number from 1 to 9** (representing the 3×3 grid) and press their player button:
  - Enter position in the **Player 1** input → click **Player 1** to place **X**
  - Enter position in the **Player 2** input → click **Player 2** to place **O**
- The app checks win conditions after each move.
- **RE-PLAY** clears the board for a new game.
- **STOP** exits the program.

### siCalculator (Simple Interest)
Enter:
- **Principal**
- **Rate**
- **Time**

Then press **Calculate** (button) to compute:
- **Simple Interest** = (Principal × Rate × Time) / 100
- **Total Amount** = Principal + Simple Interest

### simpleScientificCalculator (Scientific Calculator)
A Swing-based calculator supporting:
- Basic operations: `+`, `-`, `*`, `/`, `%`, decimal `.`
- Sign toggle: `+/-`
- Delete / clear: `DEL`, `AC`
- Scientific functions: `sin`, `cos`, `tan`, `sinh`, `cosh`, `tanh`, `log`, `exp`, `sqrt`
- Powers: `x^2`, `x^3`, `x^y`
- Reciprocal: `1/x`
- Factorial: `n!`

---

## Notes

- These are classic **NetBeans-generated Swing forms** (`.form` files) plus the corresponding `.java` files.
- If you open the projects in a different NetBeans version or JDK, you may be prompted to upgrade project metadata — that’s normal.
