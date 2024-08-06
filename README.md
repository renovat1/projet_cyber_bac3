Projet VPN
Sur un environnement Linux Debian virtualisé, vous allez installer un VPN et le sécuriser.
Partie 1
Installez OpenVPN et générez les clés et les certificats nécessaires pour configurer le
serveur VPN. Vous pouvez utiliser l&#39;outil easy-rsa qui est fourni avec OpenVPN pour le
faire. Suivez les instructions pour générer les clés et les certificats.
Ensuite, vous devrez configurer le serveur OpenVPN: créez un fichier de configuration
pour le serveur et spécifiez les paramètres nécessaires pour permettre à deux
utilisateurs de se connecter.
Pour sécuriser le VPN, vous devrez activer un cryptage fort. OpenVPN supporte
plusieurs algorithmes de cryptage, tels que AES et Blowfish. Choisissez un algorithme
de cryptage considéré comme sûr.
Enfin, lancez le serveur OpenVPN en exécutant la commande appropriée. Vous devriez
maintenant être en mesure de vous connecter au VPN à partir d&#39;autres appareils.

Partie 2
Ajoutez le service VPN au systemd afin qu’il se lance automatiquement au démarrage
du serveur..
Configurez un firewall afin que seules les connexions HTTP soient permises aux
utilisateurs se connectant au VPN.
Partie 3
Vous pouvez également sécuriser le VPN en activant l&#39;authentification à deux facteurs.
Cela exige que les utilisateurs fournissent une forme supplémentaire d&#39;authentification,
comme un code envoyé sur leur téléphone, avant de pouvoir se connecter au VPN.
Pour activer l&#39;authentification à deux facteurs, vous devrez utiliser un logiciel tel que
Google Authenticator ou Duo. Suivez les instructions pour le configurer.
