# Inexor Data Files

This repository contains all data for [Inexor](https://github.com/sauerbraten-fork/inexor).
It is intended as the core package, featuring up our main depencies in a few ~100MB.

## Licensing
A big problem we had to deal with when forking off Sauerbraten has been licensing.
This is why we decided to introduce a strict policy as you can find in [our wiki](https://github.com/sauerbraten-fork/inexor-data/wiki/License-Policy).


## How does the repo work?
The repo is splitted into packages, which may contain:
* maps
* textures
* sounds
* models
* and any additional content needed

A package will be documented using our package.json system - a example can be found below.
```json
{
    "title": "Package Title",
    "author": {
		"name": "Package Author"
		"email": "package@auth.or" 
	},
    "date": {
        "release": "package release date",
        "alpha": "package alpha date"
    },
    "license": "package license",
    "content": {
        "maps": [
            "package map"
        ],
        "textures": {
            "package texture folder": {
                "texture.png": "Some more detail about the texture",
                "moretexture.png": ""
            }
        },
        "models": {
            "package model folder": {
                "model.png": "Some more detail about the model",
                "moremodel.png": ""
            }
        },
        "dependencies": {
            "textures": [
                "texture1.png",
                "texture2.png"
            ],
            "skybox": [
                "skybox1.png"
            ]
		},
		"attribute": {
			"url": "http://some.pack.age",
			"credit": "this is a nice testing package made by a bear"
		}
    }
}

```
Don't let this frighten you, there is a nice little GUI that takes care of writing the .json for you.


## How can I get involved / contribute
We're hiring anyone who want's to contribute!
Just get in contact with us, send a patch or open a issue and we'll take care of it..
