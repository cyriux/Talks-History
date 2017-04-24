# Refactorez-vos-specs.md

# Abstract

Même en agile, les spécifications vont souvent trop loin et décrivent des solutions détaillées ; toutes ces décisions prématurées contraignent l'implémentation en écartant des opportunités. Il existe un remède : refactorer les spécfications, même avant de refactorer le code.

En TDD, refactorer est l'art de restructurer le code pour le rendre plus simple, sans changer son comportement au runtime.

Le refactoring est très utile au niveau du code, et l'est encore plus quand appliqué durant l'analyse métier préalable. Nous montrerons comment la pratique du refactoring directement au niveau du domaine métier peut simplifier le problème, et par conséquent le code d'implémentation, avec moins de code à écrire et à tester, et moins de défauts.

Nous introduirons 5 patterns pour cela, tels que "Make It Systematic" et "Degenerate Case". Nous expliquerons des limites et l'état d'esprit requis. Cette approche utilisée sur plusieurs projets réels dérive en particulier de DDD et de Specs by Example.
