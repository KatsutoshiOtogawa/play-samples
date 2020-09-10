# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.134.1/containers/ubuntu/.devcontainer/base.Dockerfile
ARG VARIANT="34"
FROM fedora:${VARIANT}

# [Optional] Uncomment this section to install additional OS packages.
RUN dnf update -y && dnf install -y java-11-openjdk

# sbt install to use scala.
RUN curl https://bintray.com/sbt/rpm/rpm | tee /etc/yum.repos.d/bintray-sbt-rpm.repo \
  && dnf install -y sbt


