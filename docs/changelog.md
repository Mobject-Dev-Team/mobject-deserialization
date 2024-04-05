# Changelog

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
