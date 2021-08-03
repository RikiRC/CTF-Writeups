# hvhpgs{synt}
# Description:
CS1 ciphers go brrrrr

# Solution:
- Open and analyze attached file with ghidra - https://ghidra-sre.org
- In Main function you can find two interesting values:
  - qe_mzp_xqffqderxms_iadpe_iuft_gzpqdeoad
  - azeupqd_ftq_cgqefuaz_omz_ymotuzqe_ftuzwu_bdabaeq_fa_o
- If you look further response to the first value should be - "very funny"
- If you try to input the text that is being printed to the user ("flag_words_with_underscores_and_letters") to the program it will print "very funny" so at this point we know that "qe_mzp_xqffqderxms_iadpe_iuft_gzpqdeoad" == "flag_words_with_underscores_and_letters"
- Next function that is in that decompiled file is "rot" - rot is actually shift cipher
- If we check "qe_mzp_xqffqderxms_iadpe_iuft_gzpqdeoad" with rot14 we will get "es_and_lettersflag_words_with_underscor" at this point we see that rot14 is correct shift but still there is a little shift in string
- If we check "azeupqd_ftq_cgqefuaz_omz_ymotuzqe_ftuzwu_bdabaeq_fa_o" with rot14 we will get "onsider_the_question_can_machines_thinki_propose_to_c"
- We can just shift manually "onsider_the_question_can_machines_thinki_propose_to_c" to "i_propose_to_consider_the_question_can_machines_think" which is the flag

# Flag:
uiuctf{i_propose_to_consider_the_question_can_machines_think}
