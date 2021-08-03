# phpfuck
# Description:
i hate php

http://phpfuck.chal.uiuc.tf

# Solution:
- Go to the - http://phpfuck.chal.uiuc.tf - on the top of the site you will see:
  - *<?php
    // Flag is inside ./flag.php :)
    ($x=str_replace("`","",strval($_REQUEST["x"])))&&strlen(count_chars($x,3))<=5?print(eval("return $x;")):show_source(__FILE__)&&phpinfo();*
- As you can see flag is in flag.php so go to - http://phpfuck.chal.uiuc.tf/flag.php - and check the source of this file

# Flag:
uiuctf{pl3as3_n0_m0rE_pHpee}
