# panel-xml

## Overview

`panel-xml` is an interactive pane designed for displaying and exploring XML within [HoloViz Panel](https://panel.holoviz.org/).

It is based on [react-xml-viewer](https://github.com/alissonmbr/react-xml-viewer).

[![panel-xml](https://github.com/awesome-panel/panel-xml/blob/main/static/panel-xml.png?raw=true)](https://py.cafe/awesome.panel.org/panel-xml-editor)

### Key Features

- **Configurable Depth**: Set an initial collapsible depth for better navigation.
- **Collapse/Expand Tags**: Intuitively collapse or expand tags to streamline XML exploration.
- **Customizable Theme**: Configure the colors and appearance with a customizable theme.

## Installation

You can install `panel-xml` using `pip`:

```bash
pip install panel-xml
```

## Usage

### Basic XML Pane

Here’s how to create a simple XML pane using the `XML` widget:

```python
import panel as pn
from panel_xml import XML

pn.extension()

xml = '''
<ul>
<li>Hello</li>
<li>World</li>
</ul>
'''

XML(object=xml, depth=2).servable()
```

[Try it on PY.CAFE](https://py.cafe/snippet/panel/v1#c=H4sIABCbGmcAA41SzUrDQBB-lTCXKsRoKyoE60ERPOjFgwpNkW13alY2u-tm-hNK393ZpLEWLS2BkJn55vvZ7BLGViKkoApnPUVOGNSRKCNnMjPxtmg674tCR2vI29NjxkNnElwQmlJZc3QcOgHTjzqdTmaup_qG31rdPKDW9vqUv5r61Xot2_q0htUbmWHeIzv6xDH1mSmOJDrK-73jpEQ_EyONQQVi8Pg1VR4LNFSy8dpf5tlQa5QxVLkQqm5xKZx7UTiHdCJ0iTGgVHRvAiek5KfccRXl1oSVykol8WR2lvQuky4va1HZKUG6hBn6kBbSHruwlp4tUy5bMc9VDONcaemRQYOfCYlRicTDuZKUQ9q9OIuhUOa1Kc-b6gHVR846oVSS1yZK4y2zcv47a0gog36HQoCejBosQ5wIvACr4Sr-62KHxc0eH1fiKtje3Yx__4CEFrQtc8Ax7I--jrIvdpv4_5z5mrV7dXGIJqHnttD7RFtcUA3PKq6Pn-_iYLj6BpCXmpVQAwAA)

### Parameters

- `object`: The XML string to display in a prettified format.
- `indent_size`: The size of the indentation.
- `collapsible`: Enable collapsing/expanding tags. When collapsed, content and attributes are hidden.
- `depth`: When `collapsible` is set to `True`, this defines the initial collapsed depth. Set it to `0` for fully collapsed, or `-1` for fully expanded.
- `theme`: A dictionary to customize the theme. See the [react-xml-viewer theme documentation](https://github.com/alissonmbr/react-xml-viewer#theme-object) for details.

## XML Editor

Try out the live XML Editor [here](https://py.cafe/awesome.panel.org/panel-xml-editor) for code or [here](https://py.cafe/app/awesome.panel.org/panel-xml-editor) for the app.

[![Panel XML | Diagram Editor](https://github.com/awesome-panel/panel-xml/blob/main/static/panel-xml-editor.gif?raw=true)](https://py.cafe/awesome.panel.org/panel-xml-editor)

## Contributions

Contributions are welcome! Please submit issues or pull requests to the [GitHub repository](https://github.com/awesome-panel/panel-xml). Check out the [DEVELOPER_GUIDE](DEVELOPER_GUIDE.md) for more information.

## License

This project is licensed under the MIT License.

Start using `panel-xml` to integrate rich, interactive XML displays directly into your Python applications!
