## Key mashing (कुंजी मैशिंग) को कैप्चर करना

- पहला कदम `x` और `z` को कैप्चर करना है, और उस गति का उपयोग करना है जिस गति पर खिलाड़ी किसी वेरिएबल के आकार को नियंत्रित करने के लिए कुंजियों को दबा रहा है। ऐसा करने के लिए आपको एक ऐसे वेरिएबल की ज़रूरत होगी जिसमें अंतिम ज्ञात कुंजी दबाए जाने को संगृहीत किया जाता है। `last_key` नामक एक वेरिएबल बनाएँ और इसे `z` पर सेट करें जब हरे झंडे को क्लिक किया जाता है।
    
    ![स्क्रिप्ट](images/greenflag1.png)

- अगली स्क्रिप्ट के लिए आपको `speed` (गति) नामक एक नए वेरिएबल की ज़रूरत होगी, तो आगे बढ़ें और इसे अभी बनाएँ। इसे गेम के शुरू होने पर `0` पर सेट किया जा सकता है।
    
    ![script](images/greenflag2.png)

<!--
when green flag clicked
set [last_key v] to [z]
set [speed v] to [0]
-->

- When the `x` key is pressed, if the `last_key` is equal to `z`, then the `speed` variable can be increased and the `last_key` can be set to `x`. This will ensure that the player can't cheat and keep hitting the `x` key to make the speed increase.
    
    ![script](images/x_script.png)

- The same can be done for the `z` key. In combination, these two scripts force the player to hit the keys *alternately* in order to increase the speed variable.
    
    ![script](images/z_script.png)

- Now test your script. Click the green flag, then repeatedly press the `x` and `z` keys and watch the speed variable increase.