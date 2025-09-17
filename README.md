# devTools
-----

### **1. Installer Java (JDK)**

Spring Boot est basé sur Java. Vous avez besoin d'un JDK (Java Development Kit) pour compiler et exécuter les applications Spring Boot.

  * **Télécharger le JDK :**  https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.8%2B9/OpenJDK21U-jdk_x64_windows_hotspot_21.0.8_9.msi
  * **Installer le JDK :** Exécutez le programme d'installation et suivez les instructions.
  * **Définir la variable d'environnement `JAVA_HOME` :**
      * Recherchez "Modifier les variables d'environnement système" dans le menu Démarrer.
      * Dans l'onglet "Avancé", cliquez sur "Variables d'environnement...".
      * Sous "Variables système", cliquez sur "Nouvelle...".
      * Nom de la variable : `JAVA_HOME`.
      * Valeur de la variable : Le chemin d'accès à votre dossier JDK (par exemple, `C:\Program Files\Java\jdk-21`).
  * **Mettre à jour le `Path` :**
      * Dans "Variables système", sélectionnez la variable `Path` et cliquez sur "Modifier...".
      * Ajoutez une nouvelle entrée : `%JAVA_HOME%\bin`. Déplacez-la en haut de la liste pour vous assurer qu'elle est trouvée en premier.
  * **Vérifier l'installation :** Ouvrez une nouvelle invite de commande (`cmd`) ou PowerShell et tapez `java -version`. Vous devriez voir la version de Java installée.

-----

### **2. Installer Gradle**

Spring Boot utilise Gradle (ou Maven) pour la gestion des dépendances et la construction de projets. Bien que Gradle soit souvent inclus avec les projets Spring, il est utile de l'avoir comme outil autonome.

  * **Télécharger Gradle :** https://services.gradle.org/distributions/gradle-9.0.0-bin.zip
  * **Extraire les fichiers :** Extrayez le contenu du fichier ZIP dans un dossier de votre disque dur (par exemple, `C:\devTools\Gradle`).
  * **Définir la variable d'environnement `GRADLE_HOME` :**
      * Créez une nouvelle variable système nommée `GRADLE_HOME`.
      * Valeur de la variable : `C:\devTools\Gradle`.
  * **Mettre à jour le `Path` :**
      * Modifiez la variable `Path` et ajoutez une nouvelle entrée : `%GRADLE_HOME%\bin`.
  * **Vérifier l'installation :** Ouvrez une nouvelle invite de commande et tapez `gradle -v`. Vous devriez voir les détails de l'installation de Gradle.

-----

### **3. Installer Flutter**

Flutter est le SDK (Software Development Kit) pour le développement d'applications mobiles.
Pour l'installation suivre la documentation proposée par la communauté Flutter : https://docs.flutter.dev/get-started/install/windows/mobile

-----

### **4. Installer PostgreSQL**

  * **Télécharger le programme d'installation :** https://sbp.enterprisedb.com/getfile.jsp?fileid=1259686
  * **Exécuter le programme d'installation :** Exécutez le fichier d'installation. Laissez les options par défaut, mais assurez-vous que les composants suivants sont sélectionnés :
      * **PostgreSQL Server**
      * **pgAdmin 4** (un outil graphique très utile)
      * **Command Line Tools**
  * **Créer un mot de passe :** Le programme d'installation vous demandera de créer un mot de passe pour le super-utilisateur `postgres`. **Mémorisez ce mot de passe, car vous en aurez besoin pour vous connecter à la base de données.** . L'installateur demandera également un port (le port par défaut est 5432). Gardez-le par défaut.
  * **Créer une base de données avec pgAdmin 4 :** Une fois l'installation terminée, ouvrez **pgAdmin 4** depuis votre menu Démarrer.
      * Faites un clic droit sur **Databases** dans le panneau de gauche.
      * Sélectionnez **Create** \> **Database...**.
      * Donnez un nom à votre base de données (par exemple, `test_db`) et cliquez sur **Save**. Vous pouvez également créer un utilisateur spécifique pour votre application et lui accorder des autorisations pour une sécurité renforcée.
