# Changelog

## v0.3.0-alpha

- Integrated deserialization errors in to deserialization feedback
- Added custom deserialization error
- Added support for mobject-collections v1.3.0
- Added support for mobject-disposable v1.1.1
- Added support for mobject-enumerable v1.2.0
- Added support for mobject-errors v0.3.0
- Added support for mobject-serialization v0.5.0
- Removed mobject-json from tests and replaced with MockJsonSeralizer

## v0.2.0-alpha

- Added support for mobject-collections v1.2.0

## v0.1.0-alpha

- Initial deserializer code taken from v0.3.0
- Added I_DeserializerObjectForwardEnumerator
- Added I_DeserializerArrayForwardEnumerator
- Added DeserializerFeedback and I_DeserializerFeedback
- Added I_DeserializerFeedbackVisitor

!> This update contains the following breaking changes to the code taken from mobject-serialization v0.3.0.

- I_Deserializer additions, Must now support the following added methods.
  - GetArrayEnumerator
  - GetObjectEnumerator
  - GetObject
- Renamed the GetKey to GetKeyObject
- TryDeserializeFrom now uses an I_DeserializerFeedback to report back a reason if it fails
- Renamed TryGetObject to TryDeserializeToObject
- Renamed TryGetKeyObject to TryDeserializeKeyToObject
