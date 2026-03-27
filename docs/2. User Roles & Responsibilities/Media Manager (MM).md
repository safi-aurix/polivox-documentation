Media Managers handle audio processing tasks at two stages: initial processing of raw recordings (format conversion, normalization) and noise injection (adding synthetic background noise for data augmentation).

**Responsibilities**
- Process raw audio recordings: format conversion, level normalization, audio cleanup, mix multiple audio tracks into single audio. See [[Initial Processing]]
	- Can download and upload any single or mixed audio tracks
- Submit initially processed sessions to QC1 for quality review
- Inject synthetic noise into approved audio files for data augmentation. See [[Noise Processing]]
- Submit noise-processed sessions to QC2 for quality review
- Handle reprocessing when QC identifies issues with initial processing or noise injection

**Available Pages**

| **Page**           | **Path**          | **Purpose**                                             |
| ------------------ | ----------------- | ------------------------------------------------------- |
| Dashboard          | /dashboard        | Processing queue overview with initial and noise queues |
| Initial Processing | /media-library    | Process raw audio, view details, submit to QC1          |
| Noise Processing   | /noise-processing | Add noise to audio, view details, submit to QC2         |
