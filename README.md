<h1 align="center">Welcome to Gitbook2pdf 👋</h1>

<p>
  <a href="https://twitter.com/fuergaosi" target="_blank">
    <img alt="Twitter: fuergaosi" src="https://img.shields.io/twitter/follow/fuergaosi.svg?style=social" />
  </a>
</p>

> Simple but powerful tools for converting gitbook pages to pdf.

### 🏠 [Homepage](https://github.com/fuergaosi233/gitbook2pdf)

[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
[English](./README.md) [中文](./README_zh.md)

## Feature

- Asynchronous grab
  Use `aiohttp` to grab
  Can be in a few seconds the data capture.

- Grab the text can be replicated
  ![](./screenshots/copy-feature.png)
- Save the original directory structure
  ![](./screenshots/index.png)

- Retain the original hyperlinks

![](./screenshots/link-feature.png)

- Completely retained the original format（Use js rendered unable to retain🤷‍♂️
- Smaller storage space, 800 pages of PDF file is only 4.6 MB

### Sample files

[KubernetesHandbook.pdf](http://cdn2.xhyuan.co/KubernetesHandbook.pdf)

## Install

### Notice!

**Because it need to use weasyprint for pdf generation but pip can't complete weasyprint installation, so you need to install it manually.**
it's weasyprint [install tutorial](https://weasyprint.readthedocs.io/en/latest/install.html#linux)
If you don't want install install dependencies you can use made of su Yang [docker image](https://github.com/soulteary/docker-gitbook-pdf-generator)

```sh
pip install -r requirements.txt
```

## Usage

```sh
python gitbook.py {url}
```

## Run tests

```sh
python gitbook.py http://self-publishing.ebookchain.org
```

## Custom

Results generated by the CSS to define if you want to add other styles can modify `gitbook.css`.

## Author

👤 **fuergaosi233**

- Twitter: [@fuergaosi](https://twitter.com/fuergaosi)
  👤 **LiaoChangjiang**

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/fuergaosi233/gitbook2pdf/issues).

## Show your support

Give a ⭐️ if this project helped you!

## warning⚠️

Using `weasyprint` to generate pdf files will compare eating memory
Please pay attention to whether your own memory is enough
