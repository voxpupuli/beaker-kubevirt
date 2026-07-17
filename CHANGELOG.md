# Changelog

All notable changes to this project will be documented in this file.

## [1.0.0](https://github.com/voxpupuli/beaker-kubevirt/tree/1.0.0) (2026-07-17)

[Full Changelog](https://github.com/voxpupuli/beaker-kubevirt/compare/a388e545ac4aa46006e53f006ad5af1a243bdbbd...1.0.0)

**Closed issues:**

- Add cleanup on exit [\#10](https://github.com/voxpupuli/beaker-kubevirt/issues/10)

**Merged pull requests:**

- CI: Apply Release best practices & Set default token permission & Generate ruby matrix [\#44](https://github.com/voxpupuli/beaker-kubevirt/pull/44) ([bastelfreak](https://github.com/bastelfreak))
- Update voxpupuli-rubocop requirement from ~\> 5.0.0 to ~\> 5.2.0 [\#43](https://github.com/voxpupuli/beaker-kubevirt/pull/43) ([dependabot[bot]](https://github.com/apps/dependabot))
- CI: apply Vox Pupuli defaults [\#39](https://github.com/voxpupuli/beaker-kubevirt/pull/39) ([bastelfreak](https://github.com/bastelfreak))
- Use /portforward/\<port\>/tcp form for VMI WebSocket URL [\#38](https://github.com/voxpupuli/beaker-kubevirt/pull/38) ([jaevans](https://github.com/jaevans))
- Keep long-running SSH sessions alive past idle timeouts [\#37](https://github.com/voxpupuli/beaker-kubevirt/pull/37) ([jaevans](https://github.com/jaevans))
- Clean up port forwarder log levels and messages [\#36](https://github.com/voxpupuli/beaker-kubevirt/pull/36) ([jaevans](https://github.com/jaevans))
- Clean up DataVolumes labeled for the test group [\#35](https://github.com/voxpupuli/beaker-kubevirt/pull/35) ([jaevans](https://github.com/jaevans))
- Unlink kubeconfig-derived tempfiles at cleanup [\#34](https://github.com/voxpupuli/beaker-kubevirt/pull/34) ([jaevans](https://github.com/jaevans))
- Bound EventMachine reactor startup wait [\#33](https://github.com/voxpupuli/beaker-kubevirt/pull/33) ([jaevans](https://github.com/jaevans))
- Validate namespace and URL-encode WebSocket path segments [\#32](https://github.com/voxpupuli/beaker-kubevirt/pull/32) ([jaevans](https://github.com/jaevans))
- Sanitize hostnames before using as k8s label values [\#31](https://github.com/voxpupuli/beaker-kubevirt/pull/31) ([jaevans](https://github.com/jaevans))
- Normalize and validate kubeconfig path [\#30](https://github.com/voxpupuli/beaker-kubevirt/pull/30) ([jaevans](https://github.com/jaevans))
- Tag NodePort services with beaker/test-group for cleanup [\#29](https://github.com/voxpupuli/beaker-kubevirt/pull/29) ([jaevans](https://github.com/jaevans))
- Don't abort cluster cleanup when a port-forwarder gets stuck [\#28](https://github.com/voxpupuli/beaker-kubevirt/pull/28) ([jaevans](https://github.com/jaevans))
- Scope at\_exit cleanup suppression to this gem's own tests [\#27](https://github.com/voxpupuli/beaker-kubevirt/pull/27) ([jaevans](https://github.com/jaevans))
- Preserve existing host\['ssh'\]\['keys'\] when configuring kubevirt key [\#26](https://github.com/voxpupuli/beaker-kubevirt/pull/26) ([jaevans](https://github.com/jaevans))
- Log SSH private key basename at INFO, full path at DEBUG [\#25](https://github.com/voxpupuli/beaker-kubevirt/pull/25) ([jaevans](https://github.com/jaevans))
- Pvc namespace [\#22](https://github.com/voxpupuli/beaker-kubevirt/pull/22) ([jaevans](https://github.com/jaevans))
- Fix Windows VM OOMKills and fail fast on virt-launcher pod failure [\#21](https://github.com/voxpupuli/beaker-kubevirt/pull/21) ([jaevans](https://github.com/jaevans))
- Add Ruby 4.0 to CI test matrix [\#20](https://github.com/voxpupuli/beaker-kubevirt/pull/20) ([jaevans](https://github.com/jaevans))
- Add bug tracker URI to gemspec metadata [\#19](https://github.com/voxpupuli/beaker-kubevirt/pull/19) ([jaevans](https://github.com/jaevans))
- Add error handling for cloud-init YAML parsing [\#18](https://github.com/voxpupuli/beaker-kubevirt/pull/18) ([jaevans](https://github.com/jaevans))
- Fix SSH key path expansion [\#17](https://github.com/voxpupuli/beaker-kubevirt/pull/17) ([jaevans](https://github.com/jaevans))
- Add error handling to VM creation in provision [\#16](https://github.com/voxpupuli/beaker-kubevirt/pull/16) ([jaevans](https://github.com/jaevans))
- Remove dead code and vague TODO [\#14](https://github.com/voxpupuli/beaker-kubevirt/pull/14) ([jaevans](https://github.com/jaevans))
- Remove stale comment from CI workflow [\#13](https://github.com/voxpupuli/beaker-kubevirt/pull/13) ([jaevans](https://github.com/jaevans))
- Remove internal files and update .gitignore [\#12](https://github.com/voxpupuli/beaker-kubevirt/pull/12) ([jaevans](https://github.com/jaevans))
- Add cleanup on exit handler for hypervisor resources [\#11](https://github.com/voxpupuli/beaker-kubevirt/pull/11) ([Copilot](https://github.com/apps/copilot-swe-agent))
- Remove setting of resources on the VM spec [\#9](https://github.com/voxpupuli/beaker-kubevirt/pull/9) ([jaevans](https://github.com/jaevans))
- Enhance PVC reference handling [\#8](https://github.com/voxpupuli/beaker-kubevirt/pull/8) ([jaevans](https://github.com/jaevans))
- Prefix options with "kubevirt\_" [\#7](https://github.com/voxpupuli/beaker-kubevirt/pull/7) ([jaevans](https://github.com/jaevans))
- Improve-port-forward [\#6](https://github.com/voxpupuli/beaker-kubevirt/pull/6) ([jaevans](https://github.com/jaevans))
- Initial windows support [\#5](https://github.com/voxpupuli/beaker-kubevirt/pull/5) ([jaevans](https://github.com/jaevans))
- fix: Modify cleanup to correctly find the name in the resource metadata [\#4](https://github.com/voxpupuli/beaker-kubevirt/pull/4) ([jaevans](https://github.com/jaevans))
- Switch license from Apache-2.0 to AGPL-3.0-or-later [\#3](https://github.com/voxpupuli/beaker-kubevirt/pull/3) ([silug](https://github.com/silug))
- More functionality [\#2](https://github.com/voxpupuli/beaker-kubevirt/pull/2) ([jaevans](https://github.com/jaevans))
- Make functional [\#1](https://github.com/voxpupuli/beaker-kubevirt/pull/1) ([jaevans](https://github.com/jaevans))



\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
