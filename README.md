

# install-pinned/pyupgrade

![](https://shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)

Securely install the latest pyupgrade release from PyPI.

This action installs a pinned version of **pyupgrade** and all its dependencies,         making sure that file hashes match. Pinning your dependencies stops supply chain attacks where an adversary         replaces pyupgrade or one of its dependencies with malicious code.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
- name: Install pyupgrade from PyPI
  uses: install-pinned/pyupgrade@8c5d343729bdce257777025c251704af4babb244  # 3.0.0
```

## Alternatives

This action is a relatively simple wrapper around the fantastic [pip-tools](https://pip-tools.rtfd.io)         and is most useful if there is no existing `requirements.txt`/`poetry.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [main repository](https://github.com/install-pinned/overview) for details.

