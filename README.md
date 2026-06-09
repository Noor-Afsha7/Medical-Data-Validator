# Medical Data Validator

A simple Python project that validates medical record data using custom validation rules, regular expressions, and list comprehensions.

## Features

* Validates medical records stored as dictionaries
* Checks for missing or invalid keys
* Validates:

  * Patient IDs
  * Ages
  * Gender values
  * Diagnoses
  * Medication lists
  * Visit IDs
* Uses regex pattern matching
* Prints detailed validation error messages
* Returns `True` for valid datasets and `False` for invalid ones

---

## Technologies Used

* Python 3
* `re` module (Regular Expressions)

---

## Validation Rules

| Field           | Validation                             |
| --------------- | -------------------------------------- |
| `patient_id`    | Must be a string matching `P####`      |
| `age`           | Must be an integer and at least 18     |
| `gender`        | Must be `male` or `female`             |
| `diagnosis`     | Must be a string or `None`             |
| `medications`   | Must be a list containing only strings |
| `last_visit_id` | Must match `V####`                     |

---

## Example Output

```bash
Valid format.
```

Example invalid output:

```bash
Unexpected format 'age: sixteen' at position 1.
Unexpected format 'gender: unknown' at position 2.
```

---

## Project Structure

```bash
medical_data_validator.py
```

---

## How to Run

1. Clone the repository

```bash
git clone <your-repository-link>
```

2. Navigate to the project folder

```bash
cd medical-data-validator
```

3. Run the script

```bash
python medical_data_validator.py
```

---

## Learning Concepts Practiced

* Functions
* Dictionaries
* List comprehensions
* `all()` function
* Regular expressions
* Data validation
* Loops and conditionals
* Argument unpacking with `**kwargs`

---

## Future Improvements

* Add support for CSV or JSON files
* Export validation reports
* Add unit tests
* Build a GUI or web version
* Integrate with databases

---

## License

This project is open-source and free to use for learning purposes.
