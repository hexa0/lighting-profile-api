Although most of the code should be self explanatory since the names are verbose, this is an outline of all of the APIs you can use!

# LightingProfile:DecodeProfileDataFromInstance(profileObject: Instance | ProfileData) -> ProfileData
 - Decodes the instance representation of the ProfileData, this will do nothing if it is already a ProfileData object.
# LightingProfile:EncodeProfileDataAsInstance(profile: ProfileData) -> Configuration
 - Encodes a ProfileData object into a roblox instance that represents the ProfileData.
# LightingProfile:CreateProfileDataFromCurrentLighting() -> Configuration
 - Creates a ProfileData object from the current lighting.
# LightingProfile:CreateProfileInstanceFromCurrentLighting() -> Configuration
 - Creates an instance representing the ProfileData object of the current lighting, this is shorthand for
```luau
	LightingProfile:EncodeProfileDataAsInstance(
		LightingProfile:CreateProfileDataFromCurrentLighting()
	)
```
# LightingProfile:ApplyProfile(profile: Instance | ProfileData)
 - Applies the given profile, accepts either an instance representation of the ProfileData or the ProfileData directly.