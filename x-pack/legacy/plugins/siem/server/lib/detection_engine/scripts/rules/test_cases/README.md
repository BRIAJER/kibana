These are example POST rules that are more either Kibana UI test cases, mis-use test cases,
any generic e2e based test cases for testing different scenarios. Normally you would not
use these type of rule based messages when writing pure REST API calls. These messages are
more of what you would see "behind the scenes" when you are using Kibana UI which can
create rules with additional "meta" data or other implementation details that aren't really
a concern for a regular REST API user.

To post all of them to see in the UI, with the scripts folder as your current working directory:

```sh
./post_rule.sh ./rules/test_cases/*.json
```

To post only one at a time:

```sh
./post_rule.sh ./rules/test_cases/<filename>.json
```
