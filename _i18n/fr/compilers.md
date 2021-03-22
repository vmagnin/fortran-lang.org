---
layout: page
title: Fortran Compilers
navbar: Compilers
---

Plus d'une douzaine de compilateurs Fortran open source ou commerciaux sont 
disponibles.

## Compilateurs open source

### Compilateur GNU Fortran

Le [compilateur GNU Fortran (gfortran)](https://gcc.gnu.org/fortran/) est un
compilateur libre et open source, faisant partie de la collection de 
compilateurs GNU GCC.

La bibliothèque [OpenCoarrays](http://www.opencoarrays.org/) permet à gfortran d'implémenter les fonctionnalités de programmation parallèle du Fortran 2018, en offrant une couche d'abstraction vers différents systèmes de programmation parallèle.	

### LLVM Flang

[Flang](https://github.com/llvm/llvm-project/tree/main/flang)
est un nouveau frontal Fortran 2018 qui a été récemment
ajouté à LLVM. Il est implémenté en C++ moderne et utilise un dialecte MLIR orienté Fortran pour passer à la représentation intermédiaire LLVM IR.
Ce projet est en phase de développement actif.

### Flang classique

[Flang](https://github.com/flang-compiler/flang) est un compilateur à code 
source ouvert basé sur le compilateur commercial NVIDIA/PGI.

### LFortran

[LFortran](https://lfortran.org) est un compilateur Fortran moderne et
interactif basé sur LLVM.


## Compilateurs commerciaux

### Intel

[Intel oneAPI](https://software.intel.com/content/www/us/en/develop/tools/oneapi/all-toolkits.html) est la suite Intel de compilateurs, d'outils et de bibliothèques pour les langages Fortran, C, C++ et Python. Le Toolkit Intel oneAPI HPC fournit [deux compilateurs Fortran] (https://software.intel.com/content/www/us/en/develop/articles/intel-oneapi-fortran-compiler-release-notes.html) :
* Intel Fortran Compiler Classic (`ifort`), un compilateur mature
  implémentant intégralement la norme Fortran 2018,
* Intel Fortran Compiler Beta (`ifx`), un nouveau compilateur basé sur LLVM qui prend en charge Fortran 95 et de façon partielle les normes plus récentes.

Intel oneAPI est disponible gratuitement.
Actuellement, le compilateur est disponible pour Linux, macOS, les plates-formes Windows et les architectures x86\_64.
Un support communautaire est assuré pour la version libre sur le [forum des développeurs Intel](https://community.intel.com/t5/Intel-Fortran-Compiler/bd-p/fortran-compiler).


### NAG

Le dernier [compilateur Fortran NAG 7.0] (https://www.nag.com/nag-compiler)
offre une prise en charge étendue des fonctionnalités Fortran anciennes et modernes, y compris la programmation parallèle avec les co-tableaux, ainsi qu'une prise en charge étendue d'OpenMP.

Le compilateur implémente également une partie significative de la norme Fortran 2018 (opérations atomiques, événements et tâches, ainsi que d'autres éléments moins importants), presque toute la norme Fortran 2008, et intégralement la norme Fortran 2003 ainsi qu'OpenMP 3.1. Des outils de développement logiciel sont disponibles pour toutes les plates-formes : polisseurs de fichier source, générateur de dépendances pour les modules et les fichiers inclus, générateur de graphes d'appels, constructeur d'interfaces et unificateur de précision.

### NVIDIA
			
Les compilateurs C, C++ et Fortran du [NVIDIA HPC SDK](https://developer.nvidia.com/hpc-sdk), anciennement appelés [compilateurs PGI](https://www.pgroup.com/products/index.htm), prennent en charge l'accélération GPU des applications de modélisation et de simulation HPC codés en C++ et Fortran standards, ainsi que les directives OpenACC® et CUDA®. Des bibliothèques mathématiques accélérées par GPU maximisent les performances des algorithmes HPC courants, et des bibliothèques de communication optimisées permettent une programmation multi-GPU et sur systèmes évolutifs conforme aux standards.

Les compilateurs NVHPC sont disponibles gratuitement.
Actuellement, le compilateur est disponible pour les plates-formes Linux et pour les architectures x86\_64, ppc64le et aarch64.
Un support communautaire est assuré sur le [forum du compilateur HPC](https://forums.developer.nvidia.com/c/accelerated-computing/hpc-compilers/nvc-nvc-and-nvfortran/313).

### HPE / Cray

L'[Environnement de Compilation Cray (CCE)](https://www.cray.com/sites/default/files/SB-Cray-Programming-Environment.pdf)
est la pierre angulaire du paradigme de calcul adaptatif de Cray. Le processus de compilation du CCE se base sur une technologie Cray éprouvée qui identifie
les régions du code qui sont de type scalaire séquentielle, vectoriel parallèle, ou utilisant de nombreux fils d'exécution (multithread). Le CCE inclut des compilateurs qui exploitent automatiquement les capacités scalaires, vectorielles et multithreading du matériel Cray. Il prend en charge les langages Fortran, C et C++.


### IBM

[IBM® XL Fortran](https://www.ibm.com/us-en/marketplace/xl-fortran-linux-compiler-power)
pour Linux est un outil de programmation conforme aux standards industriels, utilisé pour développer des applications complexes en langage Fortran. Il génère du code qui exploite au mieux les capacités de la nouvelle architecture de processeur POWER9 et maximise l'utilisation de votre matériel. IBM XL Fortran pour Linux optimise votre infrastructure IBM Power Systems™ pour les grandes modélisations numériques et le calcul haute performance.

Une version communautaire des compilateurs IBM XL est disponible gratuitement. Les compilateurs sont disponibles pour Linux, les plates-formes AIX et les architectures ppc64le.

### AMD

Le système de compilation [AMD Optimizing C/C++ Compiler (AOCC)] (https://developer.amd.com/amd-aocc/) permet de générer du code haute performance de qualité. L'environnement AOCC offre de nombreuses options aux développeurs pour compiler et optimiser des applications C, C++ et Fortran pour plates-formes Linux® 32 bits et 64 bits. Le système de compilation AOCC offre des optimisations poussées, le support du multi-threading et des processeurs avec optimisation globale, vectorisation, analyses inter-procédurales, transformations de boucle,
et génération de code. AMD fournit également des bibliothèques hautement optimisées, qui exploitent au mieux chaque cœur de processeur x86. La suite de compilateurs AOCC simplifie et accélère le développement et la mise au point de vos applications x86.

Les compilateurs AOCC sont disponibles gratuitement, pour les plates-formes Linux et les architectures x86\_64.

### ARM

[Compilateur Fortran en espace utilisateur Linux] (https://developer.arm.com/tools-and-software/server-and-hpc/compile/arm-compiler-for-linux/arm-fortran-compiler).
Conçu pour le calcul haute-performance et les codes scientifiques, avec support des normes Fortran et OpenMP les plus populaires, adapté aux principales plates-formes Arm de classe serveur. Construit sur le frontal open-source Flang, et l'infrastructure d'optimisation et de génération de code LLVM. Fait partie de la collection de compilateurs Arm pour Linux.

### Absoft

[Nos compilateurs](https://www.absoft.com/products/) fournissent un code plus rapide de manière plus efficace que jamais. Pro Fortran fournit les exclusivités Absoft : équilibrage de charge AP (augmentation des performances allant jusqu'à 20 % !), AVX, OpenMP 3.1, un compilateur Fortran 95 étendu à de nombreuses fonctionnalités de F2003 et F2008, le débogueur graphique FX3, une suite d'outils natifs, la bibliothèque scientifique AMDAL HPC, et bien plus encore. De plus, Pro Fortran est le seul compilateur avec un système de visualisation rapide des données, une technologie exclusive d'Absoft pour le rendu graphique et l'affichage des données.

### Oracle / Sun

Le [compilateur Oracle C, C++, Fortran](https://www.oracle.com/application-development/technologies/developerstudio-features.html) est hautement optimisé pour les systèmes Oracle, sur site et dans le cloud.

* Technologie avancée de génération de code pour les derniers systèmes Oracle basés sur SPARC et x86
* Prise en charge des dernières normes et standards industriels, notamment C++14, C++11, C11 et OpenMP 4.0, ainsi qu'un support étendu des fonctionnalités GCC
* Analyse automatique du code pendant la compilation et protection automatique contre le débordement de la pile au moment de l'exécution


### Lahey / Fujitsu

Combinaison du compilateur 32/64 bits LGF Rainier et du compilateur classique [Lahey/Fujitsu LF95](https://lahey.com/), LF Professional v7.8 tient ses promesses ! Il implémente complètement Fortran 95/90/77 et une bonne partie de Fortran 2003 et Fortran 2008. Lahey/Fujitsu LF95 est l'un des meilleurs en terme de diagnostics de compilation.
Il comprend le compilateur GFortran avec ses fonctionnalités de parallélisation automatique, le compilateur Lahey/Fujitsu Fortran 95, le Visual Studio 2015 Shell (compatible avec VS2017), le support exclusif par Lahey de Visual Studio Fortran, la bibliothèque Winteracter WiSK Graphics, et plus encore !

### Silverfrost FTN95

[Silverfrost FTN95](https://www.silverfrost.com/) est un compilateur implémentant intégralement les normes Fortran 95, capable de produire des exécutables rapides pour les plates-formes Win32 et Microsoft .NET. FTN95 possède le meilleur système de vérifications en cours d'exécution et est livré avec de nombreux outils de développement. Sont prises en charge toutes les fonctionnalités de la norme ainsi que de nombreuses fonctionnalités non standards mais classiques, de sorte que vos projets Fortran peuvent combiner à souhait Fortran 77, Fortran 90 et Fortran 95.


### NEC

Le compilateur Fortran](https://www.nec.com/en/global/solutions/hpc/sx/tools.html) implémente la norme Fortran 2003 (ISO/IEC 1539-1:2004) ainsi que de nombreuses fonctionnalités de la norme Fortran 2008 (ISO/IEC 1539-1:2010).

## Compilateurs abandonnés

Voici une liste de compilateurs Fortran qui semblent avoir été abandonnés, et que nous n'avons donc pas répertoriés ci-dessus :

* Hewlett Packard
* Watcom
* PathScale
* G95
* Open64
* Unisys


## Remarque

Veuillez nous faire savoir si vous connaissez un compilateur qui n'est pas répertorié, ou si nous avons répertorié un compilateur dans la section *Compilateurs abandonnés* alors qu'il est bien activement maintenu.
