## Determine the Helm Deployment Phase

Determine the Deployment Phase from GH Event Name and GH Version Tag.  

- action_name == 'release' and tag not contains 'dev' --> prod
- action_name == 'release' and tag contains 'dev' --> stage
- action_name == 'push' and tag == 'main|master' --> dev
- else: ignore

