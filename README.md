## 📦 A Project Template for Self-developed Python Package

[![Package Version](https://img.shields.io/badge/Version-v1.3.0-green)](https://github.com/Ahzyuan/Python-package-template/releases/tag/v1.3.0)
[![License](https://img.shields.io/badge/License-MIT-khaki)](https://opensource.org/license/MIT)
![Pypi Template](https://img.shields.io/badge/PyPI-Package_pattern-yellow?logo=pypi&labelColor=%23FAFAFA)

[![setuptools](https://img.shields.io/badge/Build-setuptools-red)](https://github.com/pypa/setuptools)
[![Ruff](https://img.shields.io/badge/Formatter-Ruff-sienna?logo=ruff)](https://github.com/astral-sh/ruff)
[![Isort](https://img.shields.io/badge/%20Imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)

> • Planning to develop your first Python third-party package?   
> • Troubled by `setuptools`'s numerous, complex configurations?   
> • Unsure about what the structure of a project should be?    
> 𝐓𝐡𝐞𝐧 𝐲𝐨𝐮'𝐯𝐞 𝐜𝐨𝐦𝐞 𝐭𝐨 𝐭𝐡𝐞 𝐫𝐢𝐠𝐡𝐭 𝐩𝐥𝐚𝐜𝐞!

This repo provides an 𝐨𝐮𝐭-𝐨𝐟-𝐭𝐡𝐞-𝐛𝐨𝐱 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐬𝐭𝐫𝐮𝐜𝐭𝐮𝐫𝐞 𝐭𝐞𝐦𝐩𝐥𝐚𝐭𝐞 that accelerates your third-party Python package development.

## 🎯 Features

<details>
<summary>𝐀 𝐮𝐬𝐞𝐟𝐮𝐥, 𝐨𝐮𝐭-𝐨𝐟-𝐭𝐡𝐞-𝐛𝐨𝐱 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐬𝐭𝐫𝐮𝐜𝐭𝐮𝐫𝐞 that complies with software engineering specifications.</summary>

```plaix-txt
# Note: 
# the directory structure below neglects the `.github` dir and `.gitignore` file

Python-package-template/
├── tests/           # Storage unit test code
│   └── README.md    # Instructions for testing your code
├── docs/            # Store document related files
│   └── README.md    # Instructions for building document for your project
├── examples/        # Store project demo code
│   └── demo.ipynb   # Demonstration of your project
├── package-name/    # Store project code
│   ├── core.py      # Core code
│   └── __init__.py  # Package initialization file, defining copyright, version,and other information
├── LICENSE          # Project license
├── MANIFEST.in      # Describe the files included or not included in buildpackage
├── CHANGELOG.md     # Project changelog
├── README.md        # Project description
├── requirements.txt # Project dependency
├── ruff.toml        # Define rules for code style, code inspection, and importmanagement
├── packaging.sh     # Package building script
├── check_meta.sh    # Distribution metadata checking script
├── setup.cfg        # Project packaging configuration
└── setup.py         # Project packaging script
```

</details>

<details>
<summary>𝐀 𝐟𝐮𝐥𝐥𝐲 𝐜𝐨𝐧𝐟𝐢𝐠𝐮𝐫𝐞𝐝 <font color=royalblue>𝐬𝐞𝐭𝐮𝐩.𝐜𝐟𝐠</font></summary>

> 💡 Tips      
> • We use [`setup.cfg`](setup.cfg) to manage all metadata, and just keep a minimal `setup.py` to ensure editable installation supported.       
> 
> • Meanwhile, we leave all the work of code checking and import management to awesome [`Ruff`](https://github.com/astral-sh/ruff), i.e., using [`ruff.toml`](ruff.toml).

- **𝖧𝖺𝗇𝖽𝗒 𝖺𝗇𝖽 𝖼𝗈𝗆𝗉𝗋𝖾𝗁𝖾𝗇𝗌𝗂𝗏𝖾**: covers most common config items. Allows dynamic access to `version`, `README`, and project dependencies at build time.

- **𝖶𝖾𝗅𝗅 𝖼𝗈𝗆𝗆𝖾𝗇𝗍𝖾𝖽**: no need to look up [documents](https://setuptools.pypa.io/en/latest/references/keywords.html) to understand each item's meaning, comments are provided for most of them. 

</details>

<details>
<summary>𝐄𝐟𝐟𝐢𝐜𝐢𝐞𝐧𝐭 𝐚𝐧𝐝 𝐬𝐭𝐚𝐧𝐝𝐚𝐫𝐝</summary>

We use the wonderful Python linter and formatter [`Ruff`](https://github.com/astral-sh/ruff) to ensure code quality and maintainability

</details>

## 🔨 Usage

> [!IMPORTANT]   
> In demo below, we assume that your github ID is `me` and project name is `my-project`. Remember to replace them with **your own ID and project name** when using.

1. <details>
    <summary>🚀 𝐂𝐫𝐞𝐚𝐭𝐞 𝐲𝐨𝐮𝐫 𝐫𝐞𝐩𝐨</summary>
    
    Press the `Use this template` button next to `star` button,   
    so as to use this repo as a template to create your repo.
  
2. <details>
   <summary>📥 𝐂𝐥𝐨𝐧𝐞 𝐲𝐨𝐮𝐫 𝐫𝐞𝐩𝐨 𝐭𝐨 𝐥𝐨𝐜𝐚𝐥 𝐦𝐚𝐜𝐡𝐢𝐧𝐞</summary>
    
    Find new repo on your GitHub `repositories` page.    
    Pull it to your machine with `git clone`.

    ```bash
    # replace 'me' with your github ID, 
    # 'my-project' with your project name, 
    # and `MYPROJECT` with your local project folder name
    git clone https://github.com/me/my-project MYPROJECT
    ```
    </details>

3.  <details>
    <summary>✏️ 𝐑𝐞𝐧𝐚𝐦𝐞 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐟𝐨𝐥𝐝𝐞𝐫</summary>

    ```bash
    cd MYPROJECT

    # replace 'my-project' with your project name
    git mv package-name my-project
    ```

    > <details>
    > <summary>𝘯𝘰𝘸 𝘺𝘰𝘶𝘳 𝘱𝘳𝘰𝘫𝘦𝘤𝘵 𝘴𝘵𝘳𝘶𝘤𝘵𝘶𝘳𝘦 𝘴𝘩𝘰𝘶𝘭𝘥 𝘣𝘦 𝘭𝘪𝘬𝘦 𝘵𝘩𝘪𝘴</summary>
    >
    > ```
    > # Note: 
    > # the directory structure below neglects the `.github` dir and `.gitignore` file
    > 
    > MYPROJECT/
    > ├── tests/ 
    > │   └── README.md           
    > ├── docs/   
    > │   └── README.md                
    > ├── examples/  
    > │   └── demo.ipynb             
    > ├── my-project/    
    > │   ├── core.py      
    > │   └── __init__.py       
    > ├── LICENSE          
    > ├── MANIFEST.in     
    > ├── CHANGELOG.md     
    > ├── README.md        
    > ├── requirements.txt 
    > ├── ruff.toml       
    > ├── packaging.sh     
    > ├── check_meta.sh    
    > ├── setup.cfg        
    > └── setup.py         
    > ```
    > 
    > </details>
    
    </details>

4.  <details>
    <summary>📄 𝐌𝐨𝐝𝐢𝐟𝐲 𝐭𝐡𝐞 𝐟𝐨𝐥𝐥𝐨𝐰𝐢𝐧𝐠 𝐟𝐢𝐥𝐞𝐬</summary>

    <details>
    <summary>① 𝚜𝚎𝚝𝚞𝚙.𝚌𝚏𝚐 (𝚖𝚘𝚜𝚝 𝚒𝚖𝚙𝚘𝚛𝚝𝚊𝚗𝚝)</summary>

    > 💡 Tips  
    > 
    > • If your `README` is in `rst` format, you need to change `long_description_content_type` to `"text/x-rst"` instead.  
    > 
    > • If you want to create a CLI command for your package, enable `[options.entry_points]` option. See more [here](https://packaging.python.org/en/latest/guides/creating-command-line-tools/).
    > 
    > • If you want more configuration, refer to [here](https://setuptools.pypa.io/en/latest/references/keywords.html)

    **Look for the following variables in the file and modify as per comments.**

    |       Basic        |    Requirement related     | Package structure related |
    |:------------------:|:--------------------------:|:-------------------------:|
    |       `name`       |     `python_requires`      |        `packages`         |
    |     `version`      |     `install_requires`     |  `include_package_data`   |
    |      `author`      |         `exclude`          |                           |
    |   `author_email`   | `[options.extras_require]` |                           |
    |   `description`    |                            |                           |
    | `long_description` |                            |                           |
    |       `url`        |                            |                           |
    |     `keywords`     |                            |                           |
    |     `license`      |                            |                           |
    |   `classifiers`    |                            |                           |

    </details>

    <details>
    <summary> ② 𝚖𝚢-𝚙𝚛𝚘𝚓𝚎𝚌𝚝/__𝚒𝚗𝚒𝚝__.𝚙𝚢 </summary>

    - `line 2`: `<your-name>` → `me`, replace with your github ID
    - `line 8`: `0.1.0` → `0.0.1`, replace with your project initial version

    </details>

    <details>
    <summary> ③ 𝚛𝚞𝚏𝚏.𝚝𝚘𝚖𝚕 </summary>

    > • Here show the common change of `ruff.toml`  
    > • With comments in the file, you can modify everything as needed.   
    > • If you want more configuration, refer to [Ruff document](https://docs.astral.sh/ruff/)

    - `line 3`: `target-version = "py37"` → `"py310"`, replace with your target python 
    - `line 46`: `known-first-party = ["<your_package_name>"]` → `["my-project"]`, replace with your project name

    </details>

    <details>
    <summary> ④ 𝚛𝚎𝚚𝚞𝚒𝚛𝚎𝚖𝚎𝚗𝚝𝚜.𝚝𝚡𝚝 </summary>

    > Change with your project dependencies, here is an example

    ```plain-txt
    setuptools
    isort
    ruff
    opencv-python
    tqdm
    ```

    </details>

    <details>
    <summary> ⑤ 𝚁𝙴𝙰𝙳𝙼𝙴.𝚖𝚍 </summary>

    > Change with your project description. Here is an example

    ```markdown
    # 🧐 my-project

    ![Static Badge](https://img.shields.io/badge/Version-v0.0.1-green)

    ## 👋 Introduction

    This is my first Python package called `my-project`.

    ## 📦 Getting Started

    Install the package with pip: `pip install my-project`

    ## 📄 License

    This project is licensed under the MIT License, 
    see the [LICENSE.md](LICENSE.md) for details

    ## 💖 Acknowledge

    Thanks for John for his help.
    ```

    </details>


    <details>
    <summary> ⑥ 𝙻𝚒𝚌𝚎𝚗𝚜𝚎 </summary>

    > Default license is `MIT`, you can change it to other.  
    > See https://choosealicense.com/licenses/

    ```
    line 3: Copyright (c) <YEAR> <COPYRIGHT HOLDER>
    ↓
    line 3: Copyright (c) 2024 me
    ```

    </details>

    </details>

5.  <details>
    <summary>👨‍💻 𝐃𝐞𝐯𝐞𝐥𝐨𝐩 𝐲𝐨𝐮𝐫 𝐩𝐫𝐨𝐣𝐞𝐜𝐭</summary>

    > 💡 Tips    
    > • Cross-module imports can be made via `.module-name` or `my-project.module-name` in each module file.  
    > 
    > • You can test your code using `python -m my-project.<module-name>` with working directory in `MYPROJECT`.   
    > 
    > • To develop a command-line tool, add `__main__.py` in `my-project` folder. It defines logit when typing `my-project` in terminal. See more [here](https://packaging.python.org/en/latest/guides/creating-command-line-tools/)

    **Fill your logit into `my-project` folder**.

    </details>

6.  <details>
    <summary>🗳 𝐁𝐮𝐢𝐥𝐝 𝐝𝐢𝐬𝐭𝐫𝐢𝐛𝐮𝐭𝐢𝐨𝐧 𝐩𝐚𝐜𝐤𝐚𝐠𝐞𝐬</summary>

    > This step will generate `.tar.gz` source distribution file and `.whl` built distribution in new created folder `dist` .

    ```bash
    # pwd: .../MYPROJECT
    chmod +x packaging.sh

    # Assume you are using anaconda to manage your python environment
    ./packaging.sh

    # Otherwise, activate your environment and execute following command
    python -m build -v -n .
    ```

    </details>

7.  <details>
    <summary>🔍 𝐕𝐚𝐥𝐢𝐝𝐚𝐭𝐞 𝐩𝐚𝐜𝐤𝐚𝐠𝐞</summary>

    ①. 𝖵𝖺𝗅𝗂𝖽𝖺𝗍𝖾 𝖽𝗂𝗌𝗍𝗋𝗂𝖻𝗎𝗍𝗂𝗈𝗇 𝗆𝖾𝗍𝖺𝖽𝖺𝗍𝖺

    ```bash
    # pwd: .../MYPROJECT
    pip install twine

    chmod +x check_meta.sh
    ./check_meta.sh
    ```

    ②. 𝖵𝖺𝗅𝗂𝖽𝖺𝗍𝖾 `𝖬𝖠𝖭𝖨𝖥𝖤𝖲𝖳.𝗂𝗇` 𝗂𝖿 𝗒𝗈𝗎 𝗁𝖺𝗏𝖾 𝗍𝗁𝗂𝗌 𝖿𝗂𝗅𝖾.

    ```bash
    # pwd: .../MYPROJECT
    pip install check-manifest

    # command below will automatically add missing file patterns to MANIFEST.in.
    check-manifest -u -v
    ```

    ③. `𝖮𝗉𝗍𝗂𝗈𝗇` 𝖵𝖺𝗅𝗂𝖽𝖺𝗍𝖾 𝗉𝖺𝖼𝗄𝖺𝗀𝖾 𝖿𝗎𝗇𝖼𝗍𝗂𝗈𝗇𝗌
    
    ```bash
    # pwd: .../MYPROJECT
    pip install dist/*.whl
    
    # then test your package to see whether it works well.
    # this is necessary if you have create a CLI tool for your package.
    ```
    
    </details>

8.  <details>
    <summary>📢 𝐏𝐮𝐛𝐥𝐢𝐬𝐡 𝐩𝐚𝐜𝐤𝐚𝐠𝐞</summary>

    > • This step will upload your package to [`PyPI`](https://pypi.org/) or [`TestPyPI`](https://test.pypi.org/).  
    > • So firstly, you need to register an account with [`PyPI`](https://pypi.org/) or [`TestPyPI`](https://test.pypi.org/).  
    > • Also, don't forget to generate a token for uploading your package. See more [here](https://pypi.org/help/#apitoken).
    
    > 📋 **𝖲𝗎𝗀𝗀𝖾𝗌𝗍𝗂𝗈𝗇**   
    > You likely have many commits to `PyPI` or `TestPyPI` to familiarize yourself with the process. In this case, you can maintain a **forged `PyPI` server locally**, see [`🧰 Tools Recommended -> pypi-server` below](#tools-recommended).

    ```bash
    # pwd: .../MYPROJECT

    # (Option but strongly recommended) upload to testpypi firstly to see if anywhere wrong
    twine upload --repository testpypi dist/* 

    # upload to pypi
    # then everyone can install your package via `pip install my-project`
    twine upload --repository pypi dist/* 
    ```
    After executing command above, you will be asked to **enter your account token**.  

    - Sure, you can paste your token in terminal to go through the process.   
    
    - But if you are tired of doing this, you can use `.pypirc` and `keyring` to automatically access your token whenever needed. Follow the step in [`configure.pypirc and keyring 🔐` below](#tools-recommended).:

    </details>

---

> 🥳 𝗖𝗼𝗻𝗴𝗿𝗮𝘁𝘂𝗹𝗮𝘁𝗶𝗼𝗻𝘀!   
> • You have successfully published your package to `PyPI`.    
> • Now everyone can install it via `pip install my-project`   
> • To update your package to a new version, repeat steps 5 to 8 above.

## 🧰 Tools Recommended

<details>
<summary>Ⅰ 𝚙𝚢𝚙𝚒-𝚜𝚎𝚛𝚟𝚎𝚛 🖥️</summary>

> • **What is it**: A simple `PyPI` server for local use.   
> • **Highly recommended** if you are **testing your CI/CD workflow**.

You likely have many commits to `PyPI` or `TestPyPI` to familiarize yourself with publishing process. Then there exists two problems:
  
> • [`TestPyPI` / `PyPI` project size limit](https://pypi.org/help/#project-size-limit): many commits can exceed project size limit.    
> 
> • Using `TestPyPI` as the index of `pip install` is not always reliable:  especially when your package depends on some packages that are only available on `PyPI` but not on `TestPyPI`.   
> >For example, if your package `mp-project` depends on `ruff`, then `pip install mp-project -i https://test.pypi.org/simple` will fail with `ResolutionImpossible` or `Package not found` in the process of finding and downloading `ruff`, cause `ruff` is only available on `PyPI`.

To solve these problems and fully imitate the bahvior of normal `pip install` using `PyPI` index. You can deploy a local `PyPI` server with `pypi-server`.

Here is a quick guide to get started, please check its [repo](https://github.com/pypiserver/pypiserver ) for more details.


```bash

pip install pypiserver 

mkdir Path/to/store/packages  # path to store distribution packages

pypi-server run \
-i 0.0.0.0 \
-p <port> \                  # specify a port to listen
<path-to-store>/.pypiserver_pkgs\
-a . -P . &                  # disable authentication for intranet use

cat >~/.pypirc<<EOF          # add local server to .pypirc
[distutils]
index-servers =
    pypi
    testpypi
    local

[pypi]
repository: https://upload.pypi.org/legacy/

[testpypi]
repository: https://test.pypi.org/legacy/

[local]
    repository: http://0.0.0.0:7418
    username: none          # random string, not important
    password: none          # random string, not important
EOF
```

OK, then we can use commands below to upload and install packages:

```bash
# pwd: .../package project dir

# upload package to local server
twine upload --repository local dist/*

# install package from local server
pip install <package> \
--trusted-host \
--extra-index-url http://0.0.0.0:<port>/simple/ 
```

If you want to close the server, using `kill -9 "$(pgrep pypi-server)"`.

</details>

<details>
<summary>Ⅱ 𝖼𝗈𝗇𝖿𝗂𝗀𝗎𝗋𝖾 .𝚙𝚢𝚙𝚒𝚛𝚌 𝖺𝗇𝖽 𝚔𝚎𝚢𝚛𝚒𝚗𝚐 🔐</summary>

1. Configure `keyring` first

    ```bash
    pip install keyring keyrings.alt

    # if you are on Linux, execute commands below additionally.
    cat >"$(keyring diagnose | grep "config path:" | cut -d' ' -f3)"<<EOF
    [backend]
    default-keyring=keyrings.alt.file.PlaintextKeyring
    EOF

    # encrypt your pypi token 
    ## pypi
    keyring set https://upload.pypi.org/legacy/ __token__

    ## enter your pypi token when prompted

    # verify that the encrypted token has been stored
    keyring get https://upload.pypi.org/legacy/ __token__ 

    # ------------------------ same for testpypi ------------------------

    ## testpypi
    keyring set https://test.pypi.org/legacy/ __token__

    ## enter your pypi token when prompted

    # verify that the encrypted token has been stored
    keyring get https://test.pypi.org/legacy/ __token__
    ```

2. Configure `.pypirc`

    ```bash
    # refer to https://packaging.python.org/en/latest/specifications/pypirc/
    cat >~/.pypirc<<EOF
    [distutils]
    index-servers =
        pypi
        testpypi

    [pypi]
    repository = https://upload.pypi.org/legacy/

    [testpypi]
    repository = https://test.pypi.org/legacy/
    EOF

    chmod 600 ~/.pypirc
    ```

3. At this point, there is **no need** to verify your token manually when you upload packages via `twine upload`

</details>

## 🗃 Project Management 

> This section emphasizes the effective management of your project on `GitHub`.

The following files are helpful for **standardizing the process of `issue` reporting and `Pull Request`**. 

They are preset in this template repo, you can change them according to your needs

1. [`.github/CONTRIBUTING.md`](.github/CONTRIBUTING.md) : guide other to make contribution to your project. To change it, refer to [link](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors).

2. [`.github/ISSUE_TEMPLATE`](.github/ISSUE_TEMPLATE) : standardize the format of `issue` reporting. Composed of
    > Tips: Open the [`Issue page`](https://github.com/Ahzyuan/Python-package-template/issues/new/choose) to see what the template looks like.

    - [`bug_report.yml`](.github/ISSUE_TEMPLATE/bug_report.yml): template for reporting bugs.
    - [`feature_request.yml`](.github/ISSUE_TEMPLATE/feature_request.yml): template for requesting new features.
    - [`config.yml`](.github/ISSUE_TEMPLATE/config.yml): A template selector to control others' ability to initiate an `issue` without using a template.
    
    If you are to change it, refer to [link1](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository), [link2](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms) and [link3](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-githubs-form-schema).
   
1. [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) : standardize the format of `Pull Request`. To change it, refer to [link](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository).

## 📑 To Do

- [x] Add full pipeline of package development, from project preparation to maintaining.
- [ ] Add CI/CD support, such as GitHub Actions
- [ ] Add `pyproject.toml` support
- [x] Add linter

## 👀 See More

- [Setuptools User Guide](https://setuptools.pypa.io/en/latest/userguide/index.html)
- [Official Python Packaging User Guide](https://packaging.python.org)
- [Ruff document](https://docs.astral.sh/ruff/)
- [Isort document](https://pycqa.github.io/isort/index.html)

# 🧾 License

This is free and unencumbered software released into the public domain. Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.