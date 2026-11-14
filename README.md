# Camera Input LUTs

Free camera input LUTs from **IzoardPhotoVideo**, for use with DaVinci Resolve.

These LUTs convert footage recorded using specific camera colour profiles into **DaVinci Wide Gamut / DaVinci Intermediate**.

These are **technical input transforms**, not creative looks.

They're designed for use at the beginning of a colour grading workflow, allowing footage from different cameras to be graded in a common working colour space.

LUTs are named according to the transformation they provide. Names are formed as follows:

{input_format}\_to\_{output_format}\_V{version}.cube

Here, version refers to the version of the LUT, and not any version associated with the input format.

For example, version 1 of the LUT for converting Oppo O-Log to DaVinci Wide Gamut/Intermediate is named

**O-Log_to_DWI_V1.cube**

where 

{input_format} is O-Log
{output_format} is DWI, for DaVinci Wide Gamut/Intermediate
{version} is 1

## Installing the LUT in DaVinci Resolve

1. Open DaVinci Resolve.
2. Open **Project Settings → Color Management**.
3. Click **Open LUT Folder**.
4. Copy your downloaded `.cube` file into the LUT folder, preferably in a subfolder. For example, you might choose the name of the manufacturer, In this case Oppo, or perhaps `IzoardPhotoVideo`.
5. Return to Resolve and click **Update Lists** button on the Color Management Page in the **Color Management** page to refresh the available LUTs. The button is next to the one to open the LUT folder.
6. In the Color tab for the project, open the LUTs tab at the upper left of the screen, and select and apply the LUT to an appropriate input node, usually in the Group Pre-Clip area. If you don't see the new LUT, save your project and restart Resolve.

## Using the LUTs

These are **technical input transforms**, not creative looks. They are intended for a manually colour-managed
workflow where input and output transformations are managed explicitly in nodes. 

This kind of workflow is:

**Camera footage → Input LUT → Creative grading → Output transform**

The output transform converts the graded image from DWG/Intermediate to the chosen delivery format, such as Rec.709/Gamma 2.4 for SDR or Rec.2020/ST2084 for HDR.

You can find more information about using these LUTs in specific workflows by visiting the [IzoardPhotoVideo channel](https://www.youtube.com/@IzoardPhotoVideo) on YouTube

## Compatibility and limitations

- Each LUT is intended for the specified recording profile.
- A LUT does not increase the dynamic range of the original recording or recover clipped highlights.
- The LUTs are provided as `.cube` files. These are widely supported in a variety of colour grading software products and environments
- LUTs may be appropriate for only one particular colour grading product because of the output format they provide. For example, LUTs that produce DaVinci Wide Gamut/Intermediate are for use in DaVinci Resolve.
- Final results depend on the recording settings, source footage and the particular colour grading applied.

## Licence

These LUTs are intended to be free to download and use. Please refer to the [LICENSE](LICENSE.md) file for the applicable permissions and conditions.

## Tutorials and further information

These LUTs accompany the colour grading and video production tutorials published on the **IzoardPhotoVideo** YouTube channel.

[Visit IzoardPhotoVideo on YouTube](https://www.youtube.com/@IzoardPhotoVideo)

## Feedback and problems

If you encounter a specific problem with a LUT, please open a GitHub Issue in this repository, including the camera or phone you are using, and the name of the LUT.

If you have a more general question, please leave a comment on the appropriate video in the [IzoardPhotoVideo on YouTube](https://www.youtube.com/@IzoardPhotoVideo)

Include the camera model, and recording profile, for example Oppo Find X9 Pro and O-Log.