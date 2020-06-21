# Building a Social Website

> Using the Django authentication framework<br>
> Creating user registration views<br>
> Extending the user model with a custom profile model<br>
> Adding social authentication with Python Social Auth<br>

## Creating a social website project

Run the following command to create a new project::

```django
django-admin startproject bookmarks
```

The initial project structure has been created. Use the following commands to get
into your project directory and create a new application named account:

```django
cd bookmarks/
django-admin startapp account
```

```
pip install social-auth-app-django
```

```
pip install django-extensions
```

```
pip install werkzeug
pip install pyOpenSSL
```

```
pip install easy_thumbnails
```

```
pip install redis
```

```
python manage.py createsuperuser
user name: admin
email: astrid.wang1229@gmail.com
password: 12345678
```
## Features

### Go to definition in templates

Ctrl-click or press F12 on the template path in a `include` or `extends` tag
to jump to this template

### Improved syntax

- Adds the filetype `django-html` 
- Adds the filetype `django-txt` for email templates.
- Better syntax with more operators and default keywords:
  - Known default tags and filters
  - Known templatetags namespace from contrib in the {% load %} tag
  - Known keywords in tags, like: `as`, `asvar`, `with`, `trimmed`…
- Syntax highlighting everywhere in your HTML document:
  - In the HTML tag itself"
  - In the id, class or any attribute
  - In inline CSS or Javascript code

![Syntax with Gruvbox](https://github.com/vscode-django/vscode-django/raw/master/images/vscode-django-syntax-gruvbox.png)
![Syntax with Monokai](https://github.com/vscode-django/vscode-django/raw/master/images/vscode-django-syntax-monokai.png)

### Snippets

- No unnecessary new lines
- Support for selected text (when inserting snippet from the menu)
- Support for copied text

## Contributing

### Issues

Something odd? New feature request?
Please [create an issue on Github](https://github.com/vscode-django/vscode-django/issues/new).

### Setup

```bash
git clone https://github.com/vscode-django/vscode-django
cd vscode-django
npm install
code .
```

It’s better to have [TSlint](https://marketplace.visualstudio.com/items?itemName=eg2.tslint) installed.


### Launching the extension debugger

Make sure you have this snippet in `.vscode/launch.json`:

```javascript
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Extension",
      "type": "extensionHost",
      "request": "launch",
      "runtimeExecutable": "${execPath}",
      "args": [
        "--extensionDevelopmentPath=${workspaceFolder}"
      ]
    }
  ]
}
```

Press <kbd>F5</kbd> or click on Debug then Start (▶️) to launch the extension host window.

Hack around

Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>F5</kbd> or 🔄 to reload.
