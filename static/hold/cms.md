  ---
   - label: Youth Sponsor Gallery
     name: youth sponsors
     files:
       - file: content/youth/sponsors/_index.md
         label: Sponsors
         name: sponsors
         fields:
           - {label: Heading, name: heading, widget: string}
           - {label: Publish Date, name: date, widget: datetime}
           - {label: Intro, name: text, widget: text}
           - {label: Type, name: type, widget: hidden, default: youth/sponsors}
           - label: Sponsor Form Link
             name: link
             widget: object
             fields:
               - {label: Link Text, name: linkText, widget: string}
               - {label: URL, name: url, widget: string}
           - label: Images
             name: resources
             widget: list
             fields:
               - {label: Image, name: src, widget: image}
               - {label: Alt Text, name: alt, widget: string, required: false}
               - {label: Link Address, name: href, widget: string, hint: Relative address (same as title of sponsor pages)}
  ---