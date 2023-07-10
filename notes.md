This is the original mouse keys PR: https://github.com/zmkfirmware/zmk/pull/778
This is a fork that was rebased much more recently, and some additional fixes: https://github.com/urob/zmk/tree/mouse-3.2

You can test it following the instructions at https://zmk.dev/docs/features/beta-testing. Note that you have to unpair your keyboard and repair (and potentially restart your computer in between) after flashing for the mouse descriptor to work.

There is some documentation here: https://deploy-preview-778--zmk.netlify.app/docs/behaviors/mouse-emulation
See this file in lieu of the broken link on the page: https://github.com/urob/zmk/blob/mouse-3.2/app/include/dt-bindings/zmk/mouse.h
---
https://github.com/twalker/cloud-learning/blob/main/base-keymap.md
https://gist.github.com/krissen/dd27082e7ab0575619c7a31f4d2ec7ae
https://github.com/urob/zmk/blob/mouse-3.2/app/include/dt-bindings/zmk/mouse.h

---

    macros {
      ballspd: ballspd {
        label = "ballspd";
        compatible = "zmk,behavior-macro";
        #binding-cells = <0>;
        bindings
          = <&kp NLCK>
          , <&kp NLCK>
          , <&kp CLCK>
          , <&kp CLCK>
          ;
      };
    };
---
