# [Scoop](https://scoop.sh/) buckets by {{sort_order_description}}{# <!-- textlint-disable --> #}
[![Build Status](https://ci.appveyor.com/api/projects/status/github/rasa/scoop-directory?svg=true)](https://ci.appveyor.com/project/rasa/scoop-directory "Build Status") {#
#}[![Chat on Gitter](https://badges.gitter.im/lukesampson/scoop.svg)](https://gitter.im/lukesampson/scoop) {#
#}[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE) {#
#}[![Mentioned in Awesome Scoop](https://awesome.re/mentioned-badge.svg)](https://github.com/h404bi/awesome-scoop/blob/master/README.md "Awesome Scoop")

| # | [Bucket&#x25b2;](by-bucket.md) | [Apps&#x25b2;](by-apps.md) | [&#x2605;&#x25b2;](by-stars.md) | [&#x2442;&#x25b2;](by-forks.md) | [Updated&#x25b2;](by-date-updated.md) |
| :--- | :--- | ---: | ---: | ---: | ---: |
{% for repo in repos_by_score %}{#
#}|<a name="back_{{cache[repo]['id']}}" id="back_{{cache[repo]['id']}}"></a>[{{loop.index}}.](#back_{{cache[repo]['id']}}){#
#}|[__{{cache[repo]['full_name']}}__]({{cache[repo]['url']}}){{cache[repo]['cdescription']}}{#
#}|[{{cache[repo]['packages']}}](#{{cache[repo]['id']}}){#
#}|[{{cache[repo]['stars']}}]({{cache[repo]['stars_url']}}){#
#}|[{{cache[repo]['forks']}}]({{cache[repo]['forks_url']}}){#
#}|[{{cache[repo]['updated']}}]({{cache[repo]['updated_url']}} "{{cache[repo]['updated_at']}}")|
{% endfor -%}
**[Bucket&#x25b2;](by-bucket.md)** | **[Apps&#x25b2;](by-apps.md)** | **[&#x2605;&#x25b2;](by-stars.md)** | **[&#x2442;&#x25b2;](by-forks.md)** | **[Updated&#x25b2;](by-updated.md)** |

{% for repo in repos_by_name %}
## <a name="{{cache[repo]['id']}}" id="{{cache[repo]['id']}}"></a>[{{cache[repo]['full_name']}}]({{cache[repo]['url']}}) [&#x2934;](#back_{{cache[repo]['id']}})
{{cache[repo]['idescription']}}

| Name | Version | Description | License |
| :--- | :--- | :--- | :--- |
{% for entry in cache[repo]['entries'] -%}{#
#}|[{{entry['json']}}]({{entry['url']}}){#
#}|{{entry['version']}}{#
#}|{{entry['description']|e}}{#
#}|{{entry['license']}}|
{% endfor -%}{% endfor -%}

