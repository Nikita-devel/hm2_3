[Main page](https://github.com/Nikita-devel) | [Python Web Page](https://github.com/Nikita-devel/Python_Web)

# File Sorting Utility

This Python script organizes files based on their types into specific folders. It utilizes multi-processing for file factorization and multi-threading for sorting.

## Usage

1. Make sure you have Python installed on your system.

2. Clone the repository:

    ```bash
    git clone https://github.com/Nikita-devel/home_work_7.git
    ```

3. Navigate to the project directory:

    ```bash
    cd home_work_7
    ```

4. Run the script:

    ```bash
    python sort.py <path-to-directory>
    ```

    Replace `<path-to-directory>` with the path to the directory containing the files to be sorted.

5. View the organized files in the specified folders.

## Components

### `sort.py`

This script contains functions for file factorization and sorting. It includes:

- `factorize_single_process`: Single-process file factorization.
- `factorize_multi_process`: Multi-process file factorization.
- `create_queue`: Creates a multi-process queue for file factorization.
- `test_func`: Function to test the file factorization functions.

### `normalize.py`

This script defines a `Sorter` class that performs file sorting based on file extensions into specific folders. It includes:

- `on_folder`: Abstract method for handling folders.
- `move_file`: Moves a file to its corresponding folder based on its extension.
- `sort_file`: Sorts files in the specified directory into folders based on their types.
- `Worker`: A multi-threaded worker class to perform the file sorting.

## Example

```python
if __name__ == "__main__":
    main()
