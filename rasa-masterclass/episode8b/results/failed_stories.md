## happy path 1 (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* greet: hello there!
    - utter_greet   <!-- predicted: find_facility_types -->
* mood_great: amazing
    - utter_happy   <!-- predicted: action_default_fallback -->


## happy path 2 (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* greet: hello there!
    - utter_greet   <!-- predicted: find_facility_types -->
* mood_great: amazing
    - utter_happy   <!-- predicted: action_default_fallback -->
* goodbye: bye-bye!
    - utter_goodbye   <!-- predicted: action_default_fallback -->


## sad path 1 (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* greet: hello
    - utter_greet   <!-- predicted: find_facility_types -->
* mood_unhappy: not good   <!-- predicted: deny: not good -->
    - utter_cheer_up   <!-- predicted: action_default_fallback -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* affirm: yes
    - utter_happy   <!-- predicted: action_default_fallback -->


## sad path 2 (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* greet: hello
    - utter_greet   <!-- predicted: find_facility_types -->
* mood_unhappy: not good   <!-- predicted: deny: not good -->
    - utter_cheer_up   <!-- predicted: action_default_fallback -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: not really   <!-- predicted: mood_unhappy: not really -->
    - utter_goodbye   <!-- predicted: action_default_fallback -->


## sad path 3 (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* greet: hi
    - utter_greet   <!-- predicted: find_facility_types -->
* mood_unhappy: very terrible
    - utter_cheer_up   <!-- predicted: action_default_fallback -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: no
    - utter_goodbye   <!-- predicted: action_default_fallback -->


## bot challenge (/tmp/tmp2ppqsmjc/ab4ad53dd2264bb383cac85e7a317100_conversation_tests.md)
* bot_challenge: are you a bot?   <!-- predicted: out_of_scope: are you a bot? -->
    - utter_iamabot   <!-- predicted: action_default_fallback -->


