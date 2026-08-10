# Lab Notes

Open [the lab reference](00_lab_reference.ipynb) first. It is a compact
decision guide that links to the worked examples in this folder. These
notebooks are a cleaned, lab-ready version of the pasted notes—not a
replacement for your original.

Each notebook follows the same lab-time workflow:

1. **I need to** — state the task in plain language.
2. **What data do I have?** — identify the type, shape, and useful details.
3. **Determine the tool** — choose the Python feature or library operation.
4. **Try it** — run a small, editable example.

## I need to → quick tool → notebook

Use the wording closest to your lab question, then click the notebook.

| I need to… | Quick tool | Open |
| --- | --- | --- |
| keep several lists or histories together | List of lists: `all_walks = []`, then `.append(one_history)` | [Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb) |
| turn nested numerical data into one object I can calculate with | `np.array(nested_list)` | [Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb) |
| get one row, value, or range from nested data | List: `data[row][column]`; NumPy: `array[row, column]`; slice: `start:end` | [Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb) |
| select a whole row or column from a NumPy array | Row: `array[row, :]`; column: `array[:, column]` | [Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb) |
| change, add, delete, or sort list values | assignment, `.append(...)`, `del`, `sorted(...)` | [Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb) |
| look up information by a meaningful name | Dictionary: `my_dict[key]` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| access data inside a dictionary within a dictionary | `my_dict[outer_key][inner_key]` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| turn a dictionary into a spreadsheet-like table | `pd.DataFrame(my_dict)` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| load, inspect, or summarize a CSV/DataFrame | `pd.read_csv(...)`, `.head()`, `.info()`, `.describe()` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| select one column, several columns, a row, or table cells | `df['column']`, `df[['a', 'b']]`, `.loc`, `.iloc` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| filter DataFrame rows using one or more conditions | `df[condition]`; combine with `&`, `|`, `~` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| clean or modify a DataFrame | `.fillna(...)`, `.rename(...)`, `.astype(...)`, `.str.upper()` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| add or remove DataFrame rows/columns | `pd.concat(...)`, `df['new'] = ...`, `.drop(...)` | [Dictionaries and pandas](05_dictionaries_and_pandas.ipynb) |
| choose between outcomes based on a condition | `if` / `elif` / `else` | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| repeat while a changing condition stays true | `while condition:` plus an update such as `lives -= 1` | [Loops and state](01_loops_and_state.ipynb) |
| repeat once for every item in a collection | `for item in collection:`; use `enumerate(...)` for position and value | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| loop through a dictionary, NumPy array, or DataFrame | `.items()`, `np.nditer(...)`, `.iterrows()` / `.apply(...)` | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| visit every node in a binary tree | Recursive DFS: base case `if node is None`, then visit children | [Trees and DFS](02_trees_and_dfs.ipynb) |
| generate a random integer, coin toss, or dice roll | `np.random.randint(low, high)` | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| simulate the same chance experiment many times | outer trial loop + list of final outcomes | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| simulate and plot many random walks | list of walks → `np.array(...)` → transpose with `.T` → `plt.plot(...)` | [NumPy random walks](03_numpy_random_walks.ipynb) |
| estimate the chance a random walk finishes at 60 or higher | simulate many walks → collect `walk[-1]` → `np.mean(final_positions >= 60)` | [NumPy random walks](03_numpy_random_walks.ipynb) |
| estimate the chance a random walk ever reaches 60 | keep each full walk → `np.mean([max(walk) >= 60 for walk in walks])` | [NumPy random walks](03_numpy_random_walks.ipynb) |
| choose a plot | Line: `plt.plot`; relationship: `plt.scatter`; distribution: `plt.hist` | [Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb) |
| label, scale, or clear a plot | `plt.xlabel`, `plt.ylabel`, `plt.title`, `plt.xscale`, `plt.clf()` | [NumPy random walks](03_numpy_random_walks.ipynb) |

## Notebook list

- [00 — Lab reference](00_lab_reference.ipynb)
- [01 — Loops and state](01_loops_and_state.ipynb)
- [02 — Trees and DFS](02_trees_and_dfs.ipynb)
- [03 — NumPy random walks](03_numpy_random_walks.ipynb)
- [04 — Lists, arrays, and indexing](04_lists_arrays_and_indexing.ipynb)
- [05 — Dictionaries and pandas](05_dictionaries_and_pandas.ipynb)
- [06 — Logic, loops, and simulation](06_logic_loops_and_simulation.ipynb)
