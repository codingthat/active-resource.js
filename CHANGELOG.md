### 0.9.0

* Republished activeresource@2.0.11 npm package as active-resource@0.9.0

### 0.9.1

* Removed promises from calls to `Association#assign(save: false)` in favor of synchronous assignment

### 0.9.2

* Added `Base#clone` to clone resources

### 0.9.3

* Added `#errors` to list of objects/properties cloned in `Base#clone`
* Added `afterRequest` callback to Resource classes

### 0.9.4

* Add change tracking to fields, with methods `resource.changed()` and `resource.changedFields()` accessible for seeing
changes to each resource
  * Add `klass().attributes()` for specifying attributes to track.
  * Relationships will automatically be tracked
* Add `CollectionResponse` object that is returned from `GET` requests to collection endpoints
  * Provides pagination helpers when response includes pagination links
* Allow `Interfaces.JsonApi` to be overridden easier by making all helper methods prototype properties

### Master

* **Breaking:** Switched from `jQuery.ajax` to `axios`, which have different promise interfaces