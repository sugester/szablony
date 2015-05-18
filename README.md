# Zmienne dostępne w szablonach stron Sugestera

```
{{title}}
{{forum_name}}
{{forum_description}}
{{forum_logo_url}}
{{path}}
{{full_path}}
{{forum_url}}
{{forum_path}}
{{system.favicon}}
{{system.meta}}
{{system.custom_css}}
{{system.head}}
{{system.admin_menu}}
{{sidebar}}
{{categories}}
{{notifications}}
{{body}}
{{feedback_status_menu}}
{{search_or_add}}
{{vendor_css.bootstrap '3.3.2'}}
{{template_css.default '1.0.0'}}

{{#if home_site}}:
  {{home_site.url}}
  {{home_site.name}} 
{{/if}}


{{#if user}}:
  {{user.login}}
  {{user.first_name}}
  {{user.last_name}}
  {{user.profile_path}}
  {{user.avatar}} 
{{/if}}

{{posts_javascript}}

{{#each posts}} 
  {{creaed_at}}
  {{title}}
  {{content}}
  {{url}}
  {{path}}
  {{vote_box}}
  {{answer}}  
  {{votes_count}}
  {{comments_count}}
  {{email}}
  {{kind}}
  {{status}}
  {{#if user}}:
    {{user.login}}
    {{user.first_name}}
    {{user.last_name}}
    {{user.profile_path}}
    {{user.avatar}} 
  {{/if}}
  {{each attachments}}
      {{file_name}}
      {{image}}
      {{url}}
      {{url_medium}}
  {{/each}}
  {{if image}} 
    {{image.url}}
    {{image.url_medium}}
  {{/if}}
  {{#if category}}:
    {{category.url}}
    {{category.name}} 
  {{/if}}
  {{#each voters}}
    {{user.profile_path}}
    {{user.login}}
  {{/each}}
  {{anonymous_votes}}
{{/each}}
{{{admin_info}}}

```
