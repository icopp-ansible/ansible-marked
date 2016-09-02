# ansible-marked

Install Marked via the Mac App Store or Homebrew Cask.

## Role Variables

* `prefer_mas_over_homebrew`: Defaults to `false`.

## Dependencies

* [icopp.mas-cli](https://github.com/icopp/ansible-mas-cli) (included as repository dependency), but only if `prefer_mas_over_homebrew` is `true`.
* [icopp.homebrew-cask](https://github.com/icopp/ansible-homebrew-cask) (included as repository dependency), but only if `prefer_mas_over_homebrew` is `false`.

## Example Playbook

```
  - hosts: all
    roles:
      - role: icopp.marked
```

```
  - hosts: all
    roles:
      - role: icopp.marked
        prefer_mas_over_homebrew: true
```

## License

MIT
