---
title: Vector3
type: datatype
---

# `Datatype.Vector3`

Used in 331 locations across the Roblox API.

## Used as Property Type

- `Class.AccessoryDescription.Position`
- `Class.AccessoryDescription.Rotation`
- `Class.AccessoryDescription.Scale`
- `Class.Accoutrement.AttachmentForward`
- `Class.Accoutrement.AttachmentPos`
- `Class.Accoutrement.AttachmentRight`
- `Class.Accoutrement.AttachmentUp`
- `Class.AirController.LinearImpulse`
- `Class.AlignOrientation.LookAtPosition`
- `Class.AlignOrientation.PrimaryAxis`
- `Class.AlignOrientation.SecondaryAxis`
- `Class.AlignPosition.MaxAxesForce`
- `Class.AlignPosition.Position`
- `Class.AngularVelocity.AngularVelocity`
- `Class.AtmosphereSensor.RelativeWindVelocity`
- `Class.Attachment.Axis`
- `Class.Attachment.Orientation`
- `Class.Attachment.Position`
- `Class.Attachment.Rotation`
- `Class.Attachment.SecondaryAxis`
- `Class.Attachment.WorldAxis`
- `Class.Attachment.WorldOrientation`
- `Class.Attachment.WorldPosition`
- `Class.Attachment.WorldRotation`
- `Class.Attachment.WorldSecondaryAxis`
- `Class.AvatarAccessoryRules.LimitBounds`
- `Class.AvatarClothingRules.LimitBounds`
- `Class.AvatarCollisionRules.SingleColliderSize`
- `Class.BasePart.AssemblyAngularVelocity`
- `Class.BasePart.AssemblyCenterOfMass`
- `Class.BasePart.AssemblyLinearVelocity`
- `Class.BasePart.CenterOfMass`
- `Class.BasePart.ExtentsSize`
- `Class.BasePart.Orientation`
- `Class.BasePart.Position`
- `Class.BasePart.RotVelocity`
- `Class.BasePart.Rotation`
- `Class.BasePart.Size`
- `Class.BasePart.Velocity`
- `Class.BillboardGui.ExtentsOffset`
- ...and 143 more

## Used as Parameter Type

- `Class.Attachment:SetAxis` (parameter `axis`)
- `Class.Attachment:SetSecondaryAxis` (parameter `axis`)
- `Class.BasePart:AngularAccelerationToTorque` (parameter `angAcceleration`)
- `Class.BasePart:AngularAccelerationToTorque` (parameter `angVelocity`)
- `Class.BasePart:ApplyAngularImpulse` (parameter `impulse`)
- `Class.BasePart:ApplyImpulse` (parameter `impulse`)
- `Class.BasePart:ApplyImpulseAtPosition` (parameter `impulse`)
- `Class.BasePart:ApplyImpulseAtPosition` (parameter `position`)
- `Class.BasePart:GetClosestPointOnSurface` (parameter `position`)
- `Class.BasePart:GetVelocityAtPosition` (parameter `position`)
- `Class.BasePart:TorqueToAngularAcceleration` (parameter `angVelocity`)
- `Class.BasePart:TorqueToAngularAcceleration` (parameter `torque`)
- `Class.Camera:WorldToScreenPoint` (parameter `worldPoint`)
- `Class.Camera:WorldToViewportPoint` (parameter `worldPoint`)
- `Class.Camera:ZoomToExtents` (parameter `boundingBoxSize`)
- `Class.DigitsRigDescription:SetFingerControl` (parameter `control`)
- `Class.DigitsRigDescription:SetFingerTip` (parameter `point`)
- `Class.Dragger:MouseDown` (parameter `pointOnMousePart`)
- `Class.EditableMesh:AddNormal` (parameter `normal`)
- `Class.EditableMesh:AddVertex` (parameter `p`)
- `Class.EditableMesh:FindClosestPointOnSurface` (parameter `point`)
- `Class.EditableMesh:FindClosestVertex` (parameter `toThisPoint`)
- `Class.EditableMesh:FindVerticesWithinSphere` (parameter `center`)
- `Class.EditableMesh:RaycastLocal` (parameter `direction`)
- `Class.EditableMesh:RaycastLocal` (parameter `origin`)
- `Class.EditableMesh:SetNormal` (parameter `normal`)
- `Class.EditableMesh:SetPosition` (parameter `p`)
- `Class.FluidForceSensor:EvaluateAsync` (parameter `angularVelocity`)
- `Class.FluidForceSensor:EvaluateAsync` (parameter `linearVelocity`)
- `Class.GuiService:GetClosestDialogToPosition` (parameter `position`)
- `Class.GuiService:GetClosestVisibleDialogToPosition` (parameter `position`)
- `Class.Humanoid:Move` (parameter `moveDirection`)
- `Class.Humanoid:MoveTo` (parameter `location`)
- `Class.HumanoidRigDescription:SetJointRangeMax` (parameter `rangeMax`)
- `Class.HumanoidRigDescription:SetJointRangeMin` (parameter `rangeMin`)
- `Class.Model:MoveTo` (parameter `position`)
- `Class.Model:TranslateBy` (parameter `delta`)
- `Class.Model:move` (parameter `location`)
- `Class.Model:moveTo` (parameter `location`)
- `Class.Noise:SampleDirectional` (parameter `direction`)
- ...and 71 more

## Used as Return Type

- `Class.Attachment:GetAxis`
- `Class.Attachment:GetSecondaryAxis`
- `Class.BasePart:AngularAccelerationToTorque`
- `Class.BasePart:GetClosestPointOnSurface`
- `Class.BasePart:GetVelocityAtPosition`
- `Class.BasePart:TorqueToAngularAcceleration`
- `Class.BaseWrap:GetCageOffset`
- `Class.BodyPosition:GetLastForce`
- `Class.BodyPosition:lastForce`
- `Class.BodyVelocity:GetLastForce`
- `Class.BodyVelocity:lastForce`
- `Class.Constraint:GetDebugAppliedForce`
- `Class.Constraint:GetDebugAppliedTorque`
- `Class.DigitsRigDescription:GetFingerControl`
- `Class.DigitsRigDescription:GetFingerTip`
- `Class.EditableMesh:GetCenter`
- `Class.EditableMesh:GetNormal`
- `Class.EditableMesh:GetPosition`
- `Class.EditableMesh:GetSize`
- `Class.Humanoid:ComputeOriginalSizeForPart`
- `Class.Humanoid:GetAccessoryHandleScale`
- `Class.Humanoid:GetMoveVelocity`
- `Class.Humanoid:GetRelativeVelocityAtFloor`
- `Class.HumanoidRigDescription:GetJointRangeMax`
- `Class.HumanoidRigDescription:GetJointRangeMin`
- `Class.Lighting:GetMoonDirection`
- `Class.Lighting:GetSunDirection`
- `Class.Model:GetExtentsSize`
- `Class.Model:GetModelSize`
- `Class.Terrain:CellCenterToWorld`
- `Class.Terrain:CellCornerToWorld`
- `Class.Terrain:WorldToCell`
- `Class.Terrain:WorldToCellPreferEmpty`
- `Class.Terrain:WorldToCellPreferSolid`
- `Class.UGCValidationService:GetLayeredClothingPostDeformationSize`
- `Class.VoxelBuffer:GetSizeInVoxels`
- `Class.WorkspaceAnnotation:GetAbsolutePosition`
