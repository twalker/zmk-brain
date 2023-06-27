
                win_layer {
// -----------------------------------------------------------------------------------------------------------------------------
// |       |          |          | VOL_UP     |          |BT_CLR   |   |         | ZOOM +| WIN U | WIN LG  |         |        |
// |       |          | PREV     | PLAY       | NEXT     |BT 0     |   |SCRNSHOT | WIN L | WIN D | WIN R   |  FULL   |        |
// |       |          |          | VOL_DN     | MUTE     |BT 1     |   |         | ZOOM -|       | WIN SM  |         |        |
//                                              |     |     |     |     |     |
                        bindings = <
         &none &none &kp C_VOL_UP &none &bt BT_CLR                           &none &kp LG(EQUAL) &kp LC(LA(UP)) &kp LC(LA(I)) &kp LC(LA(EQUAL))
   &none &none &kb C_PREV &kp C_PLAY &kp C_NEXT &bt BT_SEL 0                 &kp LS(LG(5)) &kp LC(LA(LEFT)) &kp LC(LA(DOWN)) &kp LC(LA(RIGHT)) &kp LC(LA(RET)) &none
   &none &none &none &kp C_VOL_DN &kp C_MUTE &bt BT_SEL 1                    &none &kp LG(MINUS) &none &kp LC(LA(K)) &kp LC(LA(MINUS)) &none
                        &trans     &trans      &trans       &trans        &trans      &trans
                        >;
                };
        };
