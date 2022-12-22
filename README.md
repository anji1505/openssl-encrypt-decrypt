# Openssl-Encrypt & Decrypt

## Zip folder creating:-

   * I created a one folder for couple of text files by using ``mkdir`` command. That was ``patch`` folder.
	
   * when I created patch folder, I enterd into the patch folder.
	
   * And I created couple of fies like `f1.txt`, `f2.txt`, `f3.txt`.
	
   * I created zip for `patch` folder by using ``sudo zip patch.zip patch .`` this command.

   * At that time I got one zip file that was ``patch.zip``

      ![Screenshot_20221222_071816](https://user-images.githubusercontent.com/116748521/209148025-00581745-f622-4bca-9abf-344f47db6fb1.png)


## Encryption of Patch.zip folder :-

   * Whenever I got the zip file of `patch` folder, I done Encryption for `patch` folder by using below command.

      `` openssl aes-256-cbc -a -salt -pbkdf2 -in patch.zip -out patch1.zip ``

   * When I was using above command, At that time it was asking password, I gave that password.

   * At that time I got ``patch1.zip``

       ![Screenshot_20221222_073017](https://user-images.githubusercontent.com/116748521/209150356-6d7e455c-cc4e-43b2-9b7a-2b6c7b36aa96.png)
	
	
## Decryption of Patch1.zip folder :-

   * When I done ``Encrypt`` the ``patch.zip`` at that time I got ``patch1.zip``.

   * So, I ``Decrypted`` the ``patch1.zip`` by using below command.

        ``openssl aes-256-cbc -d -a -pbkdf2 -in patch1.zip -out patch2.zip``
	  
   * When I done decrypt at that time I got one more zip file taht was ``patch2.zip``
	
	   ![Screenshot_20221222_074050](https://user-images.githubusercontent.com/116748521/209152351-7cf730ab-bdcb-459c-b904-e3e8c307c022.png)

   * When ``Decryption`` done, I unziped the ``patch2.zip`` in waht am I created folder, that folder was ``sandbox`` by using ``mkdir`` command.

   * When I was unzip the ``patch2.zip`` at that time I got ``patch`` folder.

       ![Screenshot_20221222_075124](https://user-images.githubusercontent.com/116748521/209154431-9a68bd98-cc79-465b-bb6d-ba5a9dd47b05.png)

   * Finally Encryption and Decryption both were successfully done. 
