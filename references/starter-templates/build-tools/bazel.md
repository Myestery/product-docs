# Bazel

{% code lineNumbers="true" %}
```yaml
version: "3"
build:
  steps:
    - type: apt-get
      packages: ["curl", "gnupg"]
      extra_repositories:
    - type: apt-get
      packages: ["bazel"]
      extra_repositories:
        - key_url: https://bazel.build/bazel-release.pub.gpg
          repository: https://storage.googleapis.com/bazel-apt
          components:
            - jdk1.8
          distribution: stable
```
{% endcode %}
