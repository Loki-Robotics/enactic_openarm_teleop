# Upstream Tracking & Usage Workflow

This repository is a **private Loki Robotics fork** of the official **Enactic Robotics openarm_teleop** repository.  
We track upstream updates from the manufacturer while keeping Loki-specific work private.

---

## 1. Remote Setup (one time)

After cloning this private repository:

```bash
git remote add upstream https://github.com/enactic/openarm_teleop.git
git fetch upstream
git remote -v   # verify

origin    git@github.com:Loki-Robotics/enactic_openarm_teleop.git
upstream  https://github.com/enactic/openarm_teleop.git
```

## 2. Syncing From Upstream

(manufacturer → local → private Loki repo)

Rebase workflow (preferred):

```bash
git fetch upstream
git checkout main
git rebase upstream/main
git push origin main
```
# OpenArm Teleop

OpenArm supports 1:1 teleoperation from a leader arm to a follower arm in two control modes. See the [documentation](https://docs.openarm.dev/teleop/) for details.

## Related links

- 📚 Read the [documentation](https://docs.openarm.dev/teleop/)
- 💬 Join the community on [Discord](https://discord.gg/FsZaZ4z3We)
- 📬 Contact us through <openarm@enactic.ai>

## License

Licensed under the Apache License 2.0. See [LICENSE.txt](LICENSE.txt) for details.

Copyright 2025 Enactic, Inc.

## Code of Conduct

All participation in the OpenArm project is governed by our [Code of Conduct](CODE_OF_CONDUCT.md).
