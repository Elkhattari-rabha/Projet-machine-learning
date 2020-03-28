# ML-Project
Sujet: Système de détection en continu et avec précision des épisodes de FA dans PPG collectés dans un cadre de vie libre ambulatoire


Difficulté et complexité: manipulation de la base de données.


Introduction pour comprendre le sujet:

La fibrillation auriculaire (FA) est l'arythmie cardiaque la plus courante et un facteur de risque d'accident vasculaire cérébral, affectant au moins 2,7 millions d'adultes aux États-Unis. Le diagnostic est habituellement effectuée par observation électrocardiogrammes (ECG) généralement mesurée avec un enregistreur d'événements cardiaques, un moniteur Holter ou un patch de poitrine. Cependant, ces appareils ECG ont tendance à être utilisés de manière réactive. De nombreuses occurrences de FA subclinique ou silencieuse ne sont donc pas détectées.


La photopléthysmographie (PPG) est une technologie émergente qui permet la mesure non invasive du rythme cardiaque grâce à la détection optique. Un capteur PPG détecte les variations du volume sanguin dans le lit microvasculaire des tissus à l'aide d'une lumière de faible intensité. De nos jours, de nombreux appareils portables existants sur le marché ont des capteurs PPG intégrés. La détection continue et précise de la FA à partir de PPG a le potentiel de transformer des appareils portables grand public à faible coût en outils de surveillance médicale cliniquement utiles à grande échelle. En utilisant la base de données clinician-annotated et les métriques d’évaluation(précision, recall, ROC ), on va réaliser une étude comparative pour l’évaluation ( des algorithmes d’apprentissage automatique suivants : DNN et KNN.


Comment utilisr ce projet:

1: déplacer la base de données "trainingset.mat" vers votre drive dans un chemin précis, dans notre cas, nous l'avons placé comme suit: "Mon Drive/notre base de données/trainingset.mat/" (la base de données est sous forme d'un fichier matlab qui contient des données médicales).


2: cliquez sur "open in colab" qui est notre platforme d'execution puisque on a pas de machines performantes pour ce travail.


3: éxecuter le 1er code qui sert à synchroniser notre platforme (google colab) avec Google drive qui contient la base de données et faire entrer le code d'autorisation donné lors de cette opération.


4: faire executer le 2ème code qui sert a uploader la base de dooonées de 'Google drive', si ca marche pas vous devez modifier dans le code le chemin (data_path1='/content/drive/My Drive/notre base de données/' et dataset =loadmat('/content/drive/My Drive/notre base de données/' + 'trainingset.mat') ) et nous vous conseillons de faire le meme chemin pour ne pas avoir de beugs (càd, creer un dossier qui s'appelle "notre base de données" dans le dossier principale "Mon Drive" et puis déposer ici la DB).



5:executer les autres codes sans problème (sauf pour l'avant dérnier code, il se peut y avoir le problème suivant de compatibilité de versions: """"If you upgrade keras older version (e.g. 2.2.5) to 2.3.0 (or newer) which is compatible with Tensorflow 2.0, you might have such error (e.g. KeyError: 'acc'). Both acc and val_acc has been renamed to accuracy and val_accuracy respectively. Renaming them in script will solve the issue"""" donc soit utiliser "acc" soit "accuray"


Pour toute information sur le code, veillez voir le "Rapport et guide de projet"
