`(27-12-24)`

## 1 - Intro : Python Language Foundation

### Q. - Why python language made? </br>
- Python is an a language that do not go with `highly theorotical while learning.`
- Python is a `Code Oriented` during <i>written</i>.
- Python are `Optimized`, `beginner friendly`, `straight forward functionality`.
- Python not include javascript like odd behaviour & it not like c++ pointer management.<br>
That of reasons python language provide 'balance' to you.

> NOTE* - Research python behind the scenes are helpful more.

----
<br>


## 2 - Best Way To Install Python

> [Python.org](https://www.python.org/)
> - Best way through learn from documentation

- Installation
- Online code
- better options to start the python.

<br>

Core python forward going to -
- Data science liblaries = Numpys, pandas, matplotlib
- Web developement = Diango, API building

<br>

### Q. - Why Python very straight forward language?
- Python can RUN anywhere, behind the scenes `compiler or s/w` run this code file it "interpret at single place community".
- Python behaviour known that could not be changed<i>(javascript have problem with behaviour change, when you run on browser or node.)</i>

After Installation python check -
- Recommanding Terminal : for windows 'gitbash'(it can use to you to run 'linux commands') => 'gitbash' provide you linux like commands use in terminal.
- Check python version : python --version
- Python identify as a best stability<i>(not breaking changes when changes version 3.11 to 3.12 to another).</i>

<br>

### Online python vs Offline python -
- For better programer you have required programming machine for python installation.
- When using online compiler for python practice,  <i>its same as you can try learn swimming without swimming pool access.</i>
  - E.g. Online compiler - OnlineGDB <i>(but you can't face problem then not become programmer).</i>
  
> NOTE* - <br>
> - In program we Not face any problems, then we not become `GOOD Programmer.`
> - Programmer `main work is Code Debugging`, not is a code writter.

<br>

Using Google Colab -
- better for online save code on cloud.
- Better way to view code output.
- Recommanding - Core Python installation & Using VS Code

Use Anaconda 2 versions (almost are notebooks) -
- conda is user friendly for libraries & output better for visualization, AI.
- all conda used for research oriented work.
- conda & mincoda are platform for code writting.
   - full-fledged Anaconda
   - Miniconda

 <br>
 
### Steps in VS Code -
- 1] Drag & drop empty folder in VS Code

- 2] Python naming convention - 
  - python as it self scripting language & also work as full fledged.
  - python community prefer underscore for name of file.
    - E.g. hello_world.py
```python
  print("chai aur python") # chai aur python
```

- 3] Open terminal in python (`in bash`) : Ctrl + ~
- 4] Run : `python 01_basics/hello_chai.py`

  
> NOTE* - Run successfully shows all work correct & in system all files installed safely.


### Stands out some questions after write below code example -

- Make file hello_chai.py

```python
# hello_chai.py
print("chai aur python")

def chai(n):
      print(n)

chai("lemon tea")
```

- Make another file chai.py

```python
# chai.py
# method call from this chai.py

from hello_chai import chai
chai("ginger tea")
```

- After running 2 files below question stand out - 
#### Q. - Why python automatic create `__pycache__` folder & whats work of `__pycache__` folder?


----
<br>

`(9-1-25)`

## 3 - Python inner working 

- We can solve below type of question - </br>

#### Q. - Why python automatic create `__pycache__` folder & under __pycache__  `----.pyc` file how to add it? What happen after delete it? After auto create python? our python code run without that file? 
       
### Behind the scene inner work of python - </br>

- We can use 1stly interpreter or software & whats script can we run? e.g. chai.py
- After .py file complete it's instruction python can make `Byte Code mostly are hidden`. Some case byte code are visible at import time are easily visible.
- thats reason we can seen __pycache__ folder.
- 1st time we can run code it also created but hidden.
- `----.pyc` is our main file. Thats our  `Byte Code`
  -  After python installation `Python VM` that `Python Virtual Machine` also installed.
  -  That VM as `actually run our code`.
-  Thats `Byte Code` that fetch under `Python VM` & run our code in under `Python VM`.

> NOTE* - <br>
> - While python code  running <i>not used of any thread, loops, queue</i>.
> - Simple creates `Byte Code` after it directly go's in `Python Virtual Machine` & `Run` python code.


1] Compile to Byte Code <i>(compile is tech jargon prnounce or technological term)</i> -
   - Actually our python code convert in byte code is `compiled down` that's `Interpretation term`.
   - `Byte Code` : `Low level code`(not a machine code) with platform independent(its only required python VM for run).
   - `Byte Code` : runs faster. becz, checks, syntax, parsing are done mostly(not 100% done but mostly done) that reasons <b>Byte Code faster run as compared to script</b>.
     - That's reasons <b>python prefer Byte codes</b>.
   - Byte code is `----.pyc` --> that acutally our `Compiled python`.
   - `Compiled python` : is also called as `Frozon Binaries`.
   - Frozon Binaries -
     - `Frozon Binaries` is not mean that --> `----.pyc`(platform independent byte code) not to used directly to run on Windows or MAC, that is differnt step.
     - Becz, that's step is final output. that time also required `Frozon Binaries` but, with us we also required `independent machines` that also produces .exe like code & in python option are also available that create .exe code.
     - That's major role of  `Frozon Binaries`.

2] `__pycache__` -
  - Sometime when we write softwares that time `__pycache__` is delete & reconstruct & also make its version.
  - When many time we can make changes in code, that not to go on our main folder becz, `at main more file is not good`.
  - That's reason of files organization by python created system folder(`__pycache__`.) that useful for python.
  - `__pycache__` : that folder indicates that `they are useful for python internal working uses`.

> NOTE* -  That's indicates importance for python internal or programmer also feed for python.

3] Source Change & Python Version - 
  - hello_chai. cpython-312.pyc
  - While changes our source code programming language use diffing algorithm (means difference finding algorithm).
  - Diffing algorithm that compare `old source .pyc to new source code .pyc` what changes only from it (not completely newly created).
  - Only changes are goes on `new .pyc` file. i.e. similar of GIT only push files changed source code.
  - `Python Version` : cpython(standard python cpython interpretation), when created .pyc is importance of python version.
  - `cpython-312.pyc` : that python 3.12 version is currently in system, that naming created by logically.
  - That means our python `byte code` build on `version 3.12` that used `cpython` of standard python that form came is .pyc `Frozon Binaries`.

- That `.pyc` files are works only for imported files & not for top level files(top level means all over under folder only 1 file present & we not used any importing).
- For top level files(only 1 file) we not required high level optimization.
<br>

`(27-1-25)`


#### PVM (Python Virtual Machine) -
- 




