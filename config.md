# JS Configurations

Hey, this is my js configs for projects

## First Step

Let's install ESLint in our project

```bash
yarn add eslint -D
```

and now lets start the eslint =)

```bash
yarn eslint --init
```

## Second Step

Here we gonna choose ur choices for config the project, this is MY settings, **copy for ur own risk =)**
<img src="./assets/first.png">

if ~~for gods sake pls no~~ u are using the old javascript features, u can use the option **CommomJS**
<img src="./assets/second.png">
Choose the framework of ur preference here ~~remember angular is bad and for this he is not here~~ _just a joke_
<img src="./assets/third.png">

Choose the platform here **use space for mark/unmark the option**
<img src="./assets/fourth.png">

I use this option for use the AirBNB style guide
<img src="./assets/fifth.png">
<img src="./assets/sixth.png">

this option is w/e, made ur favorite, i like JS <3
<img src="./assets/seventh.png">

**PRESS YES MA BOY**
<img src="./assets/eighth.png">

## Third Step

#### Install ESlint Plugin and Prettier Plugin

<img src="./assets/eslint.png">
<img src="./assets/prettier.png">

## Fourth Step

This options is for enable eslint for this languages
<img src="./assets/settings.png">

## Fifth Step

Now we are gonna overwrite some settings in our .eslintrc.js

```bash
  rules: {
    //pluggin prettier for error
    "prettier/prettier" : "error",

    //for not use this in class
    "class-methods-use-this": "off",

    //modified params in sequelize
    "no-param-reassign": "off",

    //write variables in camelCase or not
    camelcase: "off",

    //enable unused vars
    "no-unused-vars": ["error", { argsIgnorePattern: "next" }]
  }
```

And now lets add prettier dependecies

```bash
yarn add prettier eslint-config-prettier -D
yarn add prettier eslint-plugin-prettier -D
```

## Sixth Step

Lets make a file called ".prettierrc"

put this settings there

```bash
{
  "singleQuote": true,
  "trailingComma": "es5"
}

```

Its Over boys, THX =)
