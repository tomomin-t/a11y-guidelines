{%- set check_heading_level = 2 -%}
{% for check in allchecks -%}
.. _check-{{ check.id }}:

{% filter make_heading(2) -%}
チェックID：{{ check.id }}
{%- endfilter %}

対象
   {{ check.target }}
対象プラットフォーム
   {{ check.platform }}
重篤度
   {{ check.severity }}

関連ガイドライン
{%- for ref in check.gl_refs %}
   *  {{ ref.category }}： :ref:`{{ ref.glref }}`
{%- endfor %}

{{ check.check }}

{% if check.inforefs is defined -%}
{% filter make_heading(3) -%}
参考情報
{%- endfilter %}

{% for item in check.inforefs -%}
*  {{ item }}
{% endfor %}
{%- endif %}

{% if check.implementations is defined -%}
{% include 'check-implementation.rst' %}
{%- endif %}
{% if check.procedures is defined %}
{% include 'check-procedure.rst' %}
{% endif %}
{%- endfor %}
