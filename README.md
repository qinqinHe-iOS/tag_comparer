#Tag Comparer Gem

This gem provides a way to compare a list of tag versions to find out which one
is the most recent tag.

##Installation
```ruby
gem install tag_comparer # NOT UPLOADED YET!!
```

## Examples    
```ruby
TagComparer.get_latest('v1.6', 'v1.4') # returns 'v1.6'
 TagComparer.get_latest('v1','v2','v3','v3.1') # returns 'v3.1'
 TagComparer.get_latest('v1.3.1', 'v1.3') # returns 'v1.3.1'
TagComparer.get_latest('v1.3.beta10', 'v1.3.beta9') # returns 'v1.3.beta10'
TagComparer.get_latest('v1.3.rc1', 'v1.3.beta2') # returns 'v1.3.rc1'
```

## Version Prefixes/Suffixes Support
This list is in the order of most recent to oldest prefix. For example v1.3.rc1
is newer than v1.3.beta1.

- rc
- beta (or b)
- alpha (or a)


