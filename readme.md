# Palworks Animation Framework Workspace

This will contain resources for importing models into ue5 editor correctly.

### This is a very early release. Many models are not tested, and alot may be still broken. Please report all Broken Models as an Issue on this Repo, or In my discord server at: https://discord.gg/33dE4cQMA3 
You may also report if a model is working as intended. I will be updating this repo until all models are working properly. I will then move onto NPCs.


## How to import until I create an import tool:

You want to import the fbx in the directory in which the mesh is located normally. (Content\Pal\Model\Character\Monster\{monster_name}])

If there is a folder labeled 0, Import that fbx first!!!
For each model, import the FBX in Folder 1, then Import the FBX in folder 2 on top of it.

Some models have alternative meshes.
For alternate versions of the same pal you do not have to import the skeleton, You can import the base form first, then have the alternate form use the abse form's skeleton.(Default use case)

Folder 3 contains a blender file only. This is meant to be your workspace. You should be able to make changes to the model and import your changes on top of everything from here.

After import, you will have to move the Skeleton into the Skeleton Directory (Content\Pal\Model\Character\Skeleton\{monster_name}])

Rename the prefix of the Physics file from SK to PA
