# Untangling Consequences: Causality Patterns for Effective Multi-Context Design

The more you design your system into multiple Bounded Contexts, involving multiple teams, the more you’re going to face excessive coupling due to causality effects. Actions in one context often trigger consequences in others, leading to intricate dependencies, such as when updating purchase order statuses, modifying UI user journey kinematics, or undoing operations across multiple contexts.

This talk introduces unpublished modeling patterns designed to elegantly handle causality between Bounded Contexts while minimizing coupling. If your system is or is becoming modular, these patterns will prove valuable to preserve your teams' autonomy!



(NEWCRAFTS & DDD Europe 2024; Retours : "c'est exactement le problème qu'on a dans notre architecture microservices !")


# Causes & conséquences : patterns de causalité pour concevoir vos systèmes distribués

Patterns de causalité pour mieux concevoir vos systèmes distribués

Plus votre système devient modulaire, découpé en bounded contexts, plus vous êtes confronté à des couplages excessifs dus aux relations de causalité. Des actions dans un contexte, par exemple une commande d'achat ou son annulation, déclenchent ensuite des conséquences multiples dans d'autres contextes, et ce en cascade. Cela amène une grande complexité et des dépendances en partie évitables. 

Ce talk introduit des patterns de modélisation inédits pour concevoir de façon élégante les relations entre bounded contexts en suivant les relations de causalité. Nous verrons comment découpler la mise à jour d'un status client, comment réduire le "passe-plat" de données entre services, et des pistes pour simplifier les conséquences d'un changement ou d'une annulation de commande avec le paiement et la logistique, par exemple. Si votre système est ou devient modulaire, ces patterns seront précieux pour préserver l'autonomie de vos équipes !
