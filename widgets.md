# Widgets

## Spotify Large

#### Widget Code
```html
<iframe
    src="https://linkgames.de/api/v3/widget/{your_id}?type=spotify_large"
    width="600"
    height="150"
    allowtransparency="true"
    frameborder="0"
/>
```

#### Queries

| ?type= | `spotify_large` || ?language= | `en`, `de`, `tr` or `fr` || ?theme= | `light` or `dark` |
|--------|-----------------||------------|--------------------------||---------|-------------------|
| **?logo=** | **`true` or blank** || **?background=** | **`hex color`** |

> **Required Queries:** `?type=` <br>
> `?logo=` query removes `"Listening on Spotify"` text and adds a small logo.

#### Photos
![light](https://cdn.linkgames.de/assets/Spotify_large_normal.png)
![dark](https://cdn.linkgames.de/assets/Spotify_large_dark.png)

---

## Spotify Small

#### Widget Code
```html
<iframe
    src="https://linkgames.de/api/v3/widget/{your_id}?type=spotify_small"
    width="150"
    height="150"
    allowtransparency="true"
    frameborder="0"
/>
```

#### Queries

| ?type= | `spotify_small` || **?background=** | **`hex color`** || ?theme= | `light` or `dark` |
|--------|-----------------||------------------|---------------------||---------|-------------------|

> **Required Queries:** `?type=`

#### Photos
![light](https://cdn.linkgames.de/assets/Spotify_small_normal.png)
![dark](https://cdn.linkgames.de/assets/Spotify_small_dark.png)

---

## Spotify Mini

#### Widget Code
```html
<iframe
    src="https://linkgames.de/api/v3/widget/{your_id}?type=spotify_mini"
    width="300"
    height="60"
    allowtransparency="true"
    frameborder="0"
/>
```

#### Queries

| ?type= | `spotify_small` || **?background=** | **`hex color`** || ?theme= | `light` or `dark` |
|--------|-----------------||------------------|---------------------||---------|-------------------|
| **?size=** | **`a number` or `full`** |

> **Required Queries:** `?type=`

#### Photos
![light](https://cdn.linkgames.de/assets/Spotify_mini_normal.png)
![dark](https://cdn.linkgames.de/assets/Spotify_mini_dark.png)

---

## Visual Studio Code

#### Widget Code
```html
<iframe
    src="https://linkgames.de/api/v3/widget/{your_id}?type=vsc"
    width="600"
    height="150"
    allowtransparency="true"
    frameborder="0"
/>
```

#### Queries

| ?type= | `vsc` || ?language= | `en`, `de`, `tr` or `fr` || ?theme= | `light` or `dark` |
|--------|-----------------||------------|--------------------------||---------|-------------------|
| **?background=** | **`hex color`** |

> **Required Queries:** `?type=` <br>
> `!!! Important: This widget only works with the "Discord Presence" plugin.` <br>
> **[Click to view the plugin!](https://marketplace.visualstudio.com/items?itemName=icrawl.discord-vscode)**

#### Photos
![light](https://cdn.linkgames.de/assets/Visual_Studio_Code_normal.png)
![dark](https://cdn.linkgames.de/assets/Visual_Studio_Code_dark.png)

---

## Custom Status

#### Widget Code
```html
<iframe
    src="https://linkgames.de/api/v3/widget/{your_id}?type=status"
    width="300"
    height="100"
    allowtransparency="true"
    frameborder="0"
/>
```

#### Queries

| ?type= | `status` || ?size= | `a number` or `full` || ?theme= | `light` or `dark` |
|--------|-----------------||------------|--------------------------||---------|-------------------|
| **?background=** | **`hex color`** |

> **Required Queries:** `?type=`

#### Photos
![light](https://cdn.linkgames.de/assets/Custom_Status_normal.png)
![dark](https://cdn.linkgames.de/assets/Custom_Status_dark.png)