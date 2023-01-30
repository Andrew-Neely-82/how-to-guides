<h1><strong>Sass:</strong></h1>

### Install Sass (for first time) :

<br>

- run the following command in your terminal:

```
npm install -g sass
```

### Optional:

- Install `sass live compiler` extension from `Glenn Marks`

---



<br>

- Change your directory to the project folder

```
cd path/to/project

// you may need to use " " around the file path

cd "path/to/project"
```
<br>

- Make directories for src and dist

```
mkdir src
mkdir dist
```
<br>

- Once the directories are made, press `ctrl` + `shift` + `p` and type settings.json

<br>

- In the settings.json file, update the following:

```
    {
      "format": "expanded",
      "extensionName": ".css",

      =======================================Look for this=========================================

      "savePath": "path/to/save/file/to",

      =============================================================================================

    }
```

<br>

- Finally run the command and it should work:

```
sass --watch src:dist
```
