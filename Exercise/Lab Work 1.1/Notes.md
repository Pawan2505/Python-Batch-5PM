### **Q.1: Verify Python Installation**

* **Task**: Install Python and verify it.
* **Steps**:

  1. Download Python from [python.org](https://www.python.org/downloads/).
  2. Open **Command Prompt** or **Terminal**.
  3. Type:

     ```bash
     python --version
     ```
  4. Output should be something like:

     ```
     Python 3.12.0
     ```

---

### **Q.2: Write and Run Your First Python Script**

* **File Name**: `first_script.py`
* **Program**:

  ```python
  print("Name: Pawan Maurya")
  print("Age: 22")
  print("School: Gyan Manjari College")
  ```
* **Steps**:

  1. Open **IDLE**.
  2. Click **File > New File**.
  3. Paste the code and save as `first_script.py`.
  4. Run it using:

     * **Python Shell**: Type `python first_script.py` in the terminal.
     * **Python IDLE**: Press `F5` or choose **Run > Run Module**.

---

### **Q.3: Pattern Printing Program**

* **Pattern Output**:

  ```
  *
  * *
  * * *
  * *
  *
  ```
* **Program**:

  ```python
  n = 3  # height of the top half

  # Top half
  for i in range(1, n + 1):
      print('* ' * i)

  # Bottom half
  for i in range(n - 1, 0, -1):
      print('* ' * i)
  ```

