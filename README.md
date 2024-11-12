**Published glossary** available at: https://ooge0.github.io/glossary/

Project related information you can find in [intro.rst](docs/intro.rst)

**Project setup details**
## 1. Create and activate a new virtual environment:
<a href="#toc" style="color: green;">go to TOC.</a>

- **_Create virtual environment._**\
  Script below is creating environment with name 'env'.\
  If you want to create environment with unique name, please replace the env name using your env name in script\
  _python -m {here_is_your_venv_name} ../env_

  Working script for creating virtual env with name 'venv' is below:
* for windows-based OS
   ```shell
   python -m venv .venv
   ```
  
  then activate it
    * for unix-base
  ```shell
  source .venv/bin/activate
  ```
    * for windows
  ```shell
  .venv\Scripts\Activate
  ```

**_For deactivating created env use command_**
*
    ```shell
    deactivate
    ```


## 2. Install required packages from requirements.txt
<a href="#toc" style="color: green;">go to TOC.</a>

```shell
pip install -r requirements.txt
```

If **_requirements.txt_** file is missing request, or you have different configuration of the project after installation, please check generate new  _requirements.txt_ file using command 

```shell
pip-compile requirements.in
```
Created `requirements.txt` file will have all dependency for the project.

In case if you are using 'pip-tools' do next steps, 
1. check `requirements.in` content for preventing conflicts with existing(venv/global) configurations. 
2. compile requirements.txt by

```shell
pip-compile requirements.in
```

3. install dependencies by

```shell
pip install -r requirements.txt  
```
