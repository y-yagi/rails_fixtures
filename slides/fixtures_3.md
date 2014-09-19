### fixtureについて(3)

* fixturesにはERB記法が使える

```ruby
# tags.yml
ruby:
  name: ruby
  created_at: <%= 3.days.ago %>

<% 10.times do |i| %>
tag_<%= i %>:
  name: tag<%= i %>
<% end %>
```
こんなんがいける
