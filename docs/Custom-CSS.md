> This is an experimental feature. Its behaviour might change in the future.

### Instructions
1. Get class name of element you want to edit. For example, class of Settings Button would be: `Home_SettingsButton__Qvn8C`
2. Write custom styling for element using textarea at `/settings/css`. Most of the time you'll need to use `!important` in order to overwrite existing styles. For example, to change Settings Button from circle to square you would use:
```css
.Home_SettingsButton__Qvn8C {
  border-radius: 0 !important;
}
```
3. Save styles and reload page

### Examples
#### Change link size
```css
.AppCard_AppCardDetails__tbAhY span {
  font-size: 8px !important;
}
```

#### Change number of columns of Appilcation Grid and reduce page spacing
```css
.AppGrid_AppGrid__33iLW {
  grid-template-columns: repeat(7, 1fr) !important;
}

.Layout_Container__2Hv3J {
  padding: 20px 0 !important;
}
```

#### Add border to Input Group and turn it upside down
```css
.InputGroup_InputGroup__1Nm_2 {
  border: 5px solid red;
  transform: rotate(180deg);
}
```

### Problem with caching
Sometimes you might get custom css working fine on `ip:port` but not working on `flame.domain.tld`. Most of the time it's beacuse `flame.css` file is being cached. You have two ways of fixing it:
- Hard reload your page by pressing `Ctrl` + `F5` after making changes
- If you are using Cloudflare you can disable caching for specific files:
  - Open `Rules` tab and click `Create Page Rule` button
  - Type your flame instance url to match e.g. `flame.domain.tld/flame.css`
  - Set `Cache Level` to `Bypass`
  - Save and Deploy

![Cloudflare Example](https://i.ibb.co/JmZx0BT/cache.png)
