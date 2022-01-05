PyYAML
======

PyYAML是一套基于Python实现的全能YAML处理框架。

## 安装

您可以通过执行`python setup.py install`完成LibYAML的安装。

默认情况下，`setup.py`会检查LibYAML是否已安装，在LibYAML已安装的情况下会自动构建及安装LibYAML bindings。

如果想忽略相应的检查直接安装LibYAML bindings，可以执行以下命令：

`--with-libyaml`: `python setup.py --with-libyaml install`。

如果想关闭检查且忽略构建及安装LibYAML bindings，可以执行以下命令：

`--without-libyaml`: `python setup.py --without-libyaml install`。

当LibYAML bindings成功安装之后，你可以按照以下方式进行YAML流的加载解析：

    >>> yaml.load(stream, Loader=yaml.CLoader)
    >>> yaml.dump(data, Dumper=yaml.CDumper)

如果您不是很信任某个YAML输入流，可以通过安全模式进行加载：

    >>> yaml.safe_load(stream)

## 测试

PyYAML包含完整的测试套件，您可以通过执行 `python setup.py test`可以完成相应的测试用例的执行。

## 更多信息

* 如果您想获取更多关于PyYAML的信息，可以访问PyYAML官网[PyYAML homepage](https://github.com/yaml/pyyaml)和[PyYAML tutorial and reference](http://pyyaml.org/wiki/PyYAMLDocumentation)。
  
* 您也可以在Matrix上（https://matrix.to/#/#pyyaml:yaml.io）或者IRC #pyyaml irc.libera.chat 和PyYAML的维护人员进行讨论。
  
* 您也可以通过访问[PyYAML bug tracker](https://github.com/yaml/pyyaml/issues)来提交您发现的关于PyYAML的任何Bug或者您想增加的新特性。

## 协议

PyYAML模块由Kirill Simonov <xi@resolvent.net>编码实现，目前由YAML和Python社区负责维护。

PyYAML基于MIT协议发布，更多协议相关的内容可以访问LISENCE文件。
