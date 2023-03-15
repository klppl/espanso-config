# espanso-config

matches:

- trigger: ":shrugs"
  replace: "¯\_(ツ)_/¯"

- trigger: ":date"
  replace: "{{mydate}}"
  vars:
    - name: mydate
      type: date
      params:
        format: "%d-%m-%Y"
          
matches:
# ASCII Arrows
- triggers: [":-->", ":rarrow"]
  replace: "→"
- triggers: [":<--", ":larrow"]
  replace: "←"
- triggers: [":uarrow"]
  replace: "↑"
- triggers: [":darrow"]
  replace: "↓"
- triggers: [":lrarrow"]
  replace: "↓"

# Common Currency Symbols
- trigger: ':eur'
  replace: '€'
- trigger: ':gbp'
  replace: '£'
- trigger: ':usd'
  replace: '$'
- trigger: ':jpy'
  replace: '¥'
- trigger: ':inr'
  replace: '₹'
- trigger: ':btc'
  replace: '฿'
- trigger: ':eth'
  replace: 'Ξ'

- triggers: [':(c)', ':copyright:']
  replace: '©'
