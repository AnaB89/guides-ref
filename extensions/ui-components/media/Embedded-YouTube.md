# Embedded YouTube

This components allows you to easily embed YouTube videos both at design-time (properties view) and runtime (elements.my\_embed\_componen.embeddedVideoURL = "https://www.youtube.com/embed/...").

In designer it will not load/show the video; it just shows a logo and play button.

Some video options can be configured like autoplay, showControls, allowFullScreen ... More options (or even API/handler support) can be added in the future to the component - as needed.

## Youtube video player properties

The component has the following properties:

| Property               | Type       | Default | Description                                          |
| ---------------------- | ---------- | ------- | ---------------------------------------------------- |
| embeddedVideoURL       | String     | null    | The embedded youtube url to play in component        |
| videoWidth             | int        | 426     | The video width                                      |
| videoHeight            | int        | 240     | The video height                                     |
| allowFullScreen        | boolean    | true    | Option to allow full screen video                    |
| autoPlay               | boolean    | false   | Option to autoplay video on load                     |
| showControls           | boolean    | true    | Option to show video controls                        |
| modestBranding         | boolean    | false   | Option to remove youtube logo                        |
| showRelatedVideosAtEnd | boolean    | false   | Option to show related videos after video has played |
| styleClass             | styleclass | null    | Additional style class(es) of the component          |
| tabSeq                 | tabseq     | null    | Tab sequence number                                  |
| visible                | visible    | true    | When false component is not visible                  |
| size                   | dimension  | 426x240 | Component size                                       |
