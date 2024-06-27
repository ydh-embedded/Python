
#python
#markdown
#pdf

# Python
## Convert PDF to MarkDown

### Bug

```bash
	PS C:\Users\admin> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe
	c:/working-directory/Azure/PDF/pdfTomarkdown.py
	Traceback (most recent call last):
	  File "c:\working-directory\Azure\PDF\pdfTomarkdown.py", line 1, in <module>
    import pymupdf4llm
	ModuleNotFoundError: No module named 'pymupdf4llm'
```

.

```python
	
	import pymupdf4llm
		md_text = pymupdf4llm.to_markdown("Azure - Modul 0.pdf")
	# write markdown string to some file

		output = open("Azure - Modul 0.md", "w")
		output.write(md_text)
		output.close()

	import pymupdf4llm
		md_text = pymupdf4llm.to_markdown("Azure - Modul 1.pdf")
	# write markdown string to some file

		output = open("Azure - Modul 1.md", "w")
		output.write(md_text)
		output.close()


import pymupdf4llm

  

md_text = pymupdf4llm.to_markdown("Azure - Modul 2.pdf")

  

# write markdown string to some file

output = open("Azure - Modul 2.md", "w")

output.write(md_text)

output.close()

  

import pymupdf4llm

  

md_text = pymupdf4llm.to_markdown("Azure - Modul 3.pdf")

  

# write markdown string to some file

output = open("Azure - Modul 3.md", "w")

output.write(md_text)

output.close()

  

import pymupdf4llm

  

md_text = pymupdf4llm.to_markdown("Azure - Modul 4.pdf")

  

# write markdown string to some file

output = open("Azure - Modul 4.md", "w")

output.write(md_text)

output.close()
```

.

- beim compilieren traht ein Fehler auf 


![[Python - Bash I.png]]

```bash

PS C:\Users\admin> & C:/Users/admin/AppData/Local/Programs/Python/Python313/python.exe c:/working-directory/Azure/PDF/pdfTomarkdown.py
Traceback (most recent call last):
  File "c:\working-directory\Azure\PDF\pdfTomarkdown.py", line 1, in <module>
    import pymupdf4llm
ModuleNotFoundError: No module named 'pymupdf4llm'
PS C:\Users\admin> cd c:/working-directory/Azure/PDF/
PS C:\working-directory\Azure\PDF> ls

    Directory: C:\working-directory\Azure\PDF

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a---          26.06.2024    11:19        4916021 Azure - Modul 0.pdf
-a---          26.06.2024    11:17        1401731 Azure - Modul 1.pdf
-a---          26.06.2024    11:18        1730229 Azure - Modul 2.pdf
-a---          26.06.2024    11:17        1728692 Azure - Modul 3.pdf
-a---          26.06.2024    11:18        3599041 Azure - Modul 4.pdf
-a---          27.06.2024    10:12           1011 pdfTomarkdown.py

PS C:\working-directory\Azure\PDF> pip install wheel
Collecting wheel
  Downloading wheel-0.43.0-py3-none-any.whl.metadata (2.2 kB)
Downloading wheel-0.43.0-py3-none-any.whl (65 kB)
	   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 65.8/65.8 kB 1.2 MB/s eta 0:00:00
Installing collected packages: wheel
Successfully installed wheel-0.43.0

[notice] A new release of pip is available: 24.0 -> 24.1.1
[notice] To update, run: python.exe -m pip install --upgrade pip
PS C:\working-directory\Azure\PDF> python.exe -m pip install --upgrade pip
Requirement already satisfied: pip in c:\users\admin\appdata\local\programs\python\python313\lib\site-packages (24.0)
Collecting pip
  Downloading pip-24.1.1-py3-none-any.whl.metadata (3.6 kB)
Downloading pip-24.1.1-py3-none-any.whl (1.8 MB)
	   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.8/1.8 MB 1.3 MB/s eta 0:00:00
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 24.0
    Uninstalling pip-24.0:
      Successfully uninstalled pip-24.0
Successfully installed pip-24.1.1
PS C:\working-directory\Azure\PDF> 

```

.

- we will install: wheel

```bash
		pip install wheel
```

- we will install: update of pip

```bash
		python.exe -m pip install --upgrade pip
```


- we will install: Python Mu PDF

```bash
		pip install PyMuPDF
```

- then install paddleocr

```bash
		pip install paddleocr
```