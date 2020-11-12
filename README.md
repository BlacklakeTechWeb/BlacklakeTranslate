# Translate Extension For Blacklake

## Get Started

### you project should have a file named is .bl-custom.json, file content like

```json
  {
    "i18nKey": "0" // your i18n key
  }
```

## How To Use

### For Web

#### right click to BLTranslate or `cmd+i` (ctrl + i)

Selected text like `{text}` will wrapped with `<FormattedMessage defaultMessage={text}>`. In the meantime, select text will auto translate to all language json files.

#### right click to BLi18n or `cmd+ shift + i` (ctrl + shift + i)

Selected text like `{text}` will auto translate to all language json files.

### For App

right click to BLTranslate or `cmd+i` (ctrl + i)  
selected text like `你好` will formatted to `i18nConfigGlobal.t('${appTranslateKey}')`, the extension will find the word in all language file. if it exists,  appTranslateKey is the word key, if not , it will write a new word key to corresponding files first.  
like ``` `${user}, 你好` ``` will be formatted to `i18nConfigGlobal.w('${appTranslateKey}', { user })` with the default param `user` put in already.
