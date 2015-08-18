# toucht

Create a file from a template or update file headers.

## Install

```
npm install -g toucht
```

## Usage

```
toucht [filename]
```

toucht will create a file from a template for a given language.

To create a javascript file toucht a file with a .js file extension.

```
toucht file.js
```

Specify a language if there is no file extension or if you want to use a different template than the file extension.

```
toucht -l js file
```

OR

```
toucht -l javascript file
```

If the file alread exists toucht will update the date in the comment header of the file.

```
toucht file.js
```

Use a template that you created yourself

```
toucht -t template_file file
```

To add this template file as a permenant template

```
toucht --config template add your_lang template_file
```

To add a short name update your template.

```
toucht --config template update your_lang --short-name yl
```