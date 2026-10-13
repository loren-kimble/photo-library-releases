# Enhancement models

Photo Library downloads these the first time you sharpen a photo, and checks each against the SHA-256
below. They are the publishers' PyTorch weights converted to ONNX (with `torch.onnx.export`, opset 17;
ONNX Runtime's output matches PyTorch's within 2e-6), unchanged otherwise. They're in the release
[models-1](https://github.com/loren-kimble/photo-library-releases/releases/tag/models-1).

| File | Made from | SHA-256 | Licence |
|---|---|---|---|
| `realesrgan_x4plus.onnx` (67,051,598 bytes) | [RealESRGAN_x4plus.pth](https://github.com/xinntao/Real-ESRGAN/releases/tag/v0.1.0), Xintao Wang | `6c529aa057881dc3dbe5957035d70f1dec1ef7e48bf9ec8f913f08188e9aa3c1` | BSD-3-Clause: [LICENSE-Real-ESRGAN](LICENSE-Real-ESRGAN); network code from BasicSR, Apache-2.0: [LICENSE-BasicSR](LICENSE-BasicSR) |
| `gfpgan_1.4.onnx` (340,351,398 bytes) | [GFPGANv1.4.pth](https://github.com/TencentARC/GFPGAN/releases/tag/v1.3.0), Tencent ARC | `c25fa80ec944b998d56ea51199c84a0e24ef5106f1933ef596893c3700bf9098` | Apache-2.0, except third-party components under their own terms, some of them non-commercial (NVIDIA Source Code License-NC, CC BY-NC-SA 4.0): [LICENSE-GFPGAN](LICENSE-GFPGAN) |

The other models Photo Library uses are downloaded from their publishers: InsightFace's face models
(`buffalo_l`, released for non-commercial research use) and Google's SigLIP 2 vision model
(Apache-2.0, through the ONNX Community on Hugging Face).
