# **Print colored Numpy arrays / pandas DataFrames / Pandas Series / lists / dicts / tuples! **

```python
pip install PrettyColorPrinter
```

#### **This is everything you have to do to use PrettyColorPrinter with pandas**

```python
from PrettyColorPrinter import add_printer
add_printer() #This function will add some methods to PandasObject

#Let’s import pandas and create a DataFrame:

import pandas as pd
df=pd.read_csv(r"https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv")
```

<img title="" src="https://github.com/hansalemaos/PrettyColorPrinter/raw/main/a11.png" alt="">

**All methods added to pandas start either with:**

- **ds_** (for DataFrames and Series)

- **s_** (only for Series) 

- **d_** (only for DataFrames)

### **All methods that are added to PandasObject**

- **ds_color_print**

- **ds_color_print_all**

- **d_color_print_columns**

- **d_color_print_index**

- **ds_color_print_all_with_break**

- **ds_color_print_context**

```python
#If you want to see some examples:
from PrettyColorPrinter import print_test_from_pandas_github
print_test_from_pandas_github()

#If you need help
help(df.ds_color_print)
qq_ds_print(max_rows: int = 1000, max_colwidth: int = 300, repeat_cols: int = 70, asnumpy: bool = False, returndf: bool = False) -> Union[pandas.core.frame.DataFrame, pandas.core.series.Series, NoneType] method of pandas.core.frame.DataFrame instance
    Parameters
    ----------
    df : pd.DataFrame, pd.Series
        Array to print
    max_rows : int
        Stop printing after n lines (default is 1000)
    max_colwidth : int
        Width of each column (default is 300)
    repeat_cols : int (default is 70)
        Print columns again after n lines  (default is 70)
    asnumpy: bool (default is False)
        Converts pandas DataFrame to np before printing.
        If there are duplicated columns in a Pandas DataFrame,
        it changes to printasnp = True  (default is False)
    returndf:  bool (default is False)
        return the input DataFrame to allow chaining
```

### Using PrettyColorPrinter without pandas

**

The function **pdp** can be used without pandas.   
Doing it this way, you are not restricted to PandasObjects.

**You can print lists, dicts, tuples, np.arrays, pd.DataFrames and pd.Series**

**

```python
from PrettyColorPrinter import pdp
```

<img title="" src="https://github.com/hansalemaos/PrettyColorPrinter/raw/main/a1.png" alt="">
<img title="" src="https://github.com/hansalemaos/PrettyColorPrinter/raw/main/a2.png" alt="">
<img title="" src="https://github.com/hansalemaos/PrettyColorPrinter/raw/main/a3.png" alt="">
<img title="" src="https://github.com/hansalemaos/PrettyColorPrinter/raw/main/a5.png" alt="">
