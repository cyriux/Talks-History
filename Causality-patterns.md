# Consequences: Causality Patterns for Effective Multi-Context Design

The more you design your system into multiple Bounded Contexts, involving multiple teams, the more you’re going to face excessive coupling due to causality effects. Actions in one context often trigger consequences in others, leading to intricate dependencies, such as when updating purchase order statuses, modifying UI user journey kinematics, or undoing operations across multiple contexts.

This talk introduces unpublished modeling patterns designed to elegantly handle causality between Bounded Contexts while minimizing coupling. If your system is or is becoming modular, these patterns will prove valuable to preserve your teams' autonomy!


NEWCRAFTS & DDD Europe 2024
