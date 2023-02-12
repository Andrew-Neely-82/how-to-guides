<h1><strong>Sass :</strong></h1>

## **Install Sass (for first time) in VS Code :**

<br>

- #### Run the following command in your terminal :

```
npm install -g sass
```

### **Optional :**

- #### Install **`Live Sass Compiler`** extension from **`Glenn Marks`**

---

<br>

## **To use Sass in a project :**

<br>

- #### Change your directory to the project folder :

```
cd path/to/project

// you may need to use " " around the file path

cd "path/to/project"
```

<br>

- #### Make directories for **src** and **dist** :

```
mkdir src
mkdir dist
```

<br>

- ### The next step is if you plan on using the Sass Watch plugin, otherwise skip to one after this!
- #### Once the directories are made, press `ctrl` + `shift` + `p` and type **settings.json**. In the settings.json file, update the following :

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

- #### Finally run the command and it should work :

```
sass --watch src:dist
```

<br>

---

## **For more information on how to use Sass :**

- [Sass Documentation](https://sass-lang.com/documentation)
- [W3 Schools](https://www.w3schools.com/sass/)
- [Tutorials Point](https://www.tutorialspoint.com/sass/index.htm)
- [YouTube Tutorial by: freeCodeCamp ](https://www.youtube.com/watch?v=_a5j7KoflTs&t=1382s)
- [YouTube Tutorial by: developedbyed](https://www.youtube.com/watch?v=Zz6eOVaaelI)
