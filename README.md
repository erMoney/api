erMoney API
===========
Api to recognize face of av actress in japan.

**Version:** 1.0.0

**Contact information:**  
noda.sin@gmaill.com  

**License:** MIT

### /face:recognition
---
##### ***POST***
**Summary:** api to recognize face of av actress in japan

**Parameters**

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| body | body | Image capture of screen that user want to know name of peopoe in video. | Yes | [CaptureImage](#captureImage) |

**Responses**

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | Success to recognize | [FaceRecognitionResponse](#faceRecognitionResponse) |
| 404 | Not Found |
| 405 | Invalid input |

### Models
---

<a name="captureImage"></a>**CaptureImage**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| image | binary |  | No |

<a name="faceRecognitionResponse"></a>**FaceRecognitionResponse**  

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| face | object |  | No |