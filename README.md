# rime-double-jyutping-display

## About

This is a layout for typing in a custom Shuangpin (双拼) layout for Cantonese (粤语). It will display Mandarin pronunciations as you type Cantonese words. Tones can be entered as follows:

* Tone 1: `;`
* Tone 2: `/`
* Tone 3: `,`
* Tone 4: `x`
* Tone 5: `v`
* Tone 6: `.`


## Installing

First ensure you have plum installed. For macOS this would be:

```bash
cd ~/Library/Rime
wget https://git.io/rime-install
```

Then install dependencies and `gkovacs/rime-double-jyutping-display` using plum:

```bash
bash rime-install gkovacs/rime-double-jyutping gkovacs/rime-td-pinyin-flypy gkovacs/rime-double-jyutping-display
```

Finally edit `default.custom.yaml` and add `td_double_jyutping` to the schema list:

```bash
patch:
  schema_list:
    - schema: double_jyutping_display
```

Now reload RIME and it should appear under your layouts.
