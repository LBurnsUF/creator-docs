---
title: Instances
type: datatype
---

# Instances (DataType)

Used in 171 locations across the API.

## Used as Parameter Type

- BasePart.IntersectAsync(parts)
- BasePart.SubtractAsync(parts)
- BasePart.UnionAsync(parts)
- Camera.GetLargestCutoffDistance(ignoreList)
- Camera.GetPartsObscuringTarget(ignoreList)
- DraftsService.CommitEdits(scripts)
- DraftsService.DiscardEdits(scripts)
- DraftsService.RestoreScripts(scripts)
- DraftsService.ShowDiffsAgainstBase(scripts)
- DraftsService.ShowDiffsAgainstServer(scripts)
- DraftsService.ShowSourceDiffsAgainstCurrent(scripts)
- DraftsService.UpdateToLatestVersion(scripts)
- Dragger.MouseDown(parts)
- LanguageService.GetCapabilitiesUsedInPackageAsync(instances)
- PackageUIService.ConvertToPackageUpload(cloneInstances)
- PackageUIService.ConvertToPackageUpload(originalInstances)
- PackageUIService.OnOpenConvertToPackagePlugin(cloneInstances)
- PackageUIService.OnOpenConvertToPackagePlugin(instances)
- ParabolaAdornment.FindPartOnParabola(ignoreDescendentsTable)
- Plugin.Intersect(objects)
- Plugin.Negate(objects)
- Plugin.ProcessAssetInsertionDrag(instances)
- Plugin.Separate(objects)
- Plugin.Union(objects)
- PluginMouse.DragEnter(instances)
- PublishService.CreateAssetAndWaitForAssetId(instances)
- Selection.Add(instancesToAdd)
- Selection.Remove(instancesToRemove)
- Selection.Set(selection)
- SerializationService.SerializeInstancesAsync(inputInstances)
- ...and 34 more

## Used as Return Type

- AnnotationsService.GetAnnotationThreads
- AssetImportSession.GetKeyframeSequences
- AssetImportSession.GetKeyframeSequencesForSelectedRestPose
- AssetImportSession.GetKeyframeSequencesForSelectedRestPoseWithClip
- Attachment.GetConstraints
- AudioAnalyzer.GetConnectedWires
- AudioChannelMixer.GetConnectedWires
- AudioChannelSplitter.GetConnectedWires
- AudioChorus.GetConnectedWires
- AudioCompressor.GetConnectedWires
- AudioDeviceInput.GetConnectedWires
- AudioDeviceOutput.GetConnectedWires
- AudioDistortion.GetConnectedWires
- AudioEcho.GetConnectedWires
- AudioEmitter.GetConnectedWires
- AudioEmitter.GetInteractingListeners
- AudioEqualizer.GetConnectedWires
- AudioFader.GetConnectedWires
- AudioFilter.GetConnectedWires
- AudioFlanger.GetConnectedWires
- AudioGate.GetConnectedWires
- AudioLimiter.GetConnectedWires
- AudioListener.GetConnectedWires
- AudioListener.GetInteractingEmitters
- AudioPitchShifter.GetConnectedWires
- AudioPlayer.GetConnectedWires
- AudioRecorder.GetConnectedWires
- AudioRecorder.GetUnrecordableInstancesAsync
- AudioReverb.GetConnectedWires
- AudioSpeechToText.GetConnectedWires
- ...and 77 more
