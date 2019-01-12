IrishLAs FORKED version of realexpayments/rxp-hpp-php
=====================================================

Rationale
---------
We intend to use this with Drupal, however we get a dependency conflict when
installing realexpayments/rxp-hpp-php using composer.

- drupal core 8.6.x requires symfony/validator: ~3.4.0
- realexpayments/rxp-hpp-php requires symfony/validator: 2.7.*

Solution (our fork)
-------------------
Instead of relying on the upstream realexpayments/rxp-hpp-php, we use our own
fork to get around the dependency conflict.

We've simply REMOVED the dependency on symfony/validator, so we don't get a
complaint about the dependency conflict.

symfony/validator is still installed of course, via Drupal core's dependencies.
