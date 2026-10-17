# IMS (国際化マルチシフト)キーボード

[readme_日本語](https://github.com/pinekz/IMS_keyboard_module/blob/main/README.md)  

ver. 2.6 : 2026/10/18 - Enabled layer shifting while holding the thumb-shift key.
ver. 2.5 : 2026/10/10 - State machine implementation and process organization  
ver. 2.0 : 2026/07/26 - QMK 0.33.0  
ver. 1.0 : 2026/06/26 - QMK 0.27.0  

This is a module for Japanese "Kana" input based on QMK and Via.
It evolves the "Thumb Shift" input environment for natural Japanese typing, while providing a system that allows for free character placement using Via.
By allowing users to freely select and add shift keys to expand input layers, it provides a unique shift input system that is not limited to "Thumb Shift" alone.

## Features

1.  **Reference Language Layers**: Use this module to add reference language layers to English or other language keyboards, allowing you to freely arrange unique language characters.
    (Import custom keycodes into Via)
2.  **Symbol Visibility**: On Japanese layout (JP layout) keyboards, you can input symbols as they appear on English keyboards.
3.  **Shortcut Freedom**: You can freely use shortcut keys (combining English letters and modifier keys) and switch between English/Numbers and Symbol layers even while using a virtual language layer.
4.  **IME Transparency**: When the target language is Japanese, the module passes through the operation keys used by the IME (Input Method Editor). This enables a natural division of labor: the QMK keyboard handles "Kana" (phonetic) input, while the PC-side IME handles "Kana-Kanji" (semantic) conversion, allowing for seamless integration with existing IMEs.
5.  **IME_monitor**: By running `IME_monitor` on the PC side, you can achieve stress-free operation without mode switching errors.

## Characteristics

1.  **Via-based Customization**: Using the Via web interface, users can arrange character keys tailored to their individual needs, regardless of existing layouts.
    (Allows for the development of unique Kana layouts)
2.  **Simultaneous Press Support**: By freely arranging simultaneous press keys, users can substitute other fingers if they experience a thumb injury.
    (Enables the construction of a Japanese input system not limited to thumb shifts)
3.  **Modular Development**: The specific language sections are isolated into `language.c` and its corresponding header files to improve development efficiency.

## Implemented keyboards

[YMDK Air40](https://github.com/pinekz/qmk_firmware/tree/IMS-module/keyboards/ymdk/ymd40/air40/keymaps/via_ims_air40)  
[Keyboardio Atreus](https://github.com/pinekz/qmk_firmware/tree/IMS-module/keyboards/keyboardio/atreus/keymaps/via_ims_Atreus)  
