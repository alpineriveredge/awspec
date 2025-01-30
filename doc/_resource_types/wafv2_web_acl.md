### exist

You can set `scope` to CLOUDFRONT or REGIONAL ( default: `REGIONAL` ).

```ruby
describe wafv2_web_acl('my-wafv2-web-acl'), scope: 'REGIONAL' do
  it { should exist }
  its(:default_action) { should eq 'ALLOW' }
end
```
