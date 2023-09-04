# Exception Examples

## GoGoLoco

*GogoLoco is a large complicated project. Installing like this is confirmed to work. If you have questions about GoGoLoco ask in the [GogoLoco Discord](https://discord.gg/gogo-loco-911793727633260544).*

Simply add the desired GogoLoco prefab to your avatar as normal and add it to the list 'Exclude Objects From Renaming'

Also be sure to exclude any GoGoLoco controllers in the 'Exclude Animator Layers From Obfuscation' list!

![GoGoLoco](https://github.com/BlizzyFox/AntiRip/assets/105831522/dab03184-9473-48ee-81f8-51edbc82b328)

Kanna Note: In the exclude parameters from renaming section, it supports RegEx, you could thus use `.*(Go\/|(?i)go.*loco).*` to exclude all typical GoGoLoco parameters,

Encrypt, upload and write keys as normal. The GogoLoco prefab will be ignored during encryption and VRCFury will add it to your avatar on upload. 

## Face Tracking

*Please note VRCFaceTracking is a large complicated project. Installing like this is confirmed to work. If you have issues with face tracking contact the [VRCFaceTracking Discord](https://discord.gg/Fh4FNehzKn) This is not intended to be a guide on adding face tracking to an avatar. Just an example of one way to get it working with Kanna Protecc.*

Kanna Note: In the exclude parameters from renaming section, it supports RegEx, you could thus use `.*(FT\/|v2\/|Tracking).*` to exclude all VRCFaceTracking parameters.

[Jerry's Face tracking templates](https://github.com/Adjerry91/VRCFaceTracking-Templates) provides a VRCFury Prefab. Which template to use depends on your VRCFaceTracking setup. A detailed guide is included. Direct questions to [Jerry's Face tracking discord](https://discord.gg/yQtTsVSqx8). 

---

# Testing in Unity

Entering play mode will not decrypt the protected avatar on its own. There are many cases where users may want to test avatar features using the unity editor. [Gesture Manager](https://github.com/BlackStartx/VRC-Gesture-Manager) is the recommended way to do this. The package can be installed from their [github](https://github.com/BlackStartx/VRC-Gesture-Manager) or through the [Creator Companion](https://vcc.docs.vrchat.com/) if curated packages are enabled. 

<b>Gesture manager needs to access stored parameters in order to show the avatar as it will appear in game.</b>
*If you've not yet uploaded your avatar and written the keys this will not work. Upload and write keys first.*

1. Enable gesture manager in 'Tools -> Gesture Manager Emulator' select the game object in the Hierarchy and click the cog to edit its settings.

![Gesture Settings](https://github.com/BlizzyFox/AntiRip/assets/105831522/c3918b36-b51a-4848-be38-8c4a35d14d30)

2. In 'General Settings' If you've logged into multiple accounts you may need to ensure that 'User ID' is set to the one you uploaded your protected avatar to. Under 'Simulation Settings' you need to enable 'Load stored parameters'

![Gesturemanager2](https://github.com/BlizzyFox/AntiRip/assets/105831522/9ea380d0-6414-4b1e-ba74-cb972bfff8f4)

Entering play mode through Gesture Manager will now display your avatar as it should appear in game. If the avatar does not appear normal, its possible the avatars keys were not written. Ensure VRChat is closed and write the keys.

