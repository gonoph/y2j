# y2j
YAML to JSON (or JSON to YAML
## USAGE
**Requires: PyYAML**
You can install it like this for the current user:
* pip install -U PyYAML --user

Name the script either or both:
* y2j
* j2y

## PURPOSE
This will convert yaml or json into the other format. For Example:

```yaml
  name: Billy Holmes
  age:
    number: 100
    dogYears: true
  workHistory:
  - Red Hat
```

will be converted into (note that order is not guaranteed):

```json
  {"age": {"dogYears": true, "number": 100}, "name": "Billy Holmes", "workHistory": ["Red Hat"]}
```

which will be converted back to:

```yaml
  age:
    dogYears: true
    number: 100
  name: Billy Holmes
  workHistory:
    - Red Hat
```
