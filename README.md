## automatic compile from scss to css

#### 1. tool > build system > new build system

- make new build system file

```
{

  "cmd": ["sass", "--update", "$file:${file_path}/../css/${file_base_name}.css", "--stop-on-error", "--no-cache"],

  "osx":
  {
      "path": "/usr/local/bin:$PATH"
  },

  "windows":
  {
      "shell": "true"
  }

}
```


#### 2. install 'SublimeOnsaveBuild'

- setup 'Preferences' > 'Package Settings' > 'SublimeOnsaveBuild'

```
{
    "filename_filter": "(/|\\\\|^)(?!_)(\\w+)\\.(css|js|sass|less|scss)$",
    "build_on_save": 1
}
```

