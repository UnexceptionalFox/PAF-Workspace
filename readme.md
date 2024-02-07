# Palworks Animation Framework Workspace

This will contain resources for importing models into ue5 editor correctly.

### Please report all Broken Models as an Issue on this Repo, or In my discord server at: https://discord.gg/33dE4cQMA3 
You may also report if a model is working as intended. I will be updating this repo until all models are working properly. I will then move onto NPCs.


## How to import until I create an import tool:

You want to import the fbx in the directory in which the mesh is located normally. (Content\Pal\Model\Character\Monster\{monster_name}])

Every Monster will have a numbered list of folders with fbx files. Import the fbx files in ascending order of the folders. 1, 2, 3, 4, 5, ....
(You can drag the fbx files into the editor one after the other)
The Last Numbered folder in each monster folder contains a blender workspace. You can use this to work on the model, create animations, and make changes to the model, export to an fbx, and import on top of everything else.

Some models have alternative meshes.
For alternate versions of the same pal you do not have to import the skeleton and probably should not, You can import the base form first, then have the alternate form use the base form's skeleton.(Default use case)
In this case, you may be able to import the last fbx in the chain directly, as long as you reference the exsisting skeleton in the editor.

Again the last numbered folder in each monster directory contains a blender file only. This is meant to be your workspace. You should be able to make changes to the model and import your changes on top of everything from here.

After import, you will have to move the Skeleton into the Skeleton Directory (Content\Pal\Model\Character\Skeleton\{monster_name}])

Rename the prefix of the Physics file from SK to PA


NPCs and player models coming soon.