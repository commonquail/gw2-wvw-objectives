# GW2 WvW Objective Name API Fix

Version 1 of the official GW2 WvW [objective name API][objective-names] only
shows generic names, not actual place names. This JavaScript file works as an
alternative until ArenaNet updates the API to include more information.

The structure of objectives tries to mimic that of the official API as closely
as possible:

* `id`: The objective id
* `type`: The type of an objective by the in-game classification
* `score`: The value of this objective, generally tied to `type`
* `map`: One of the four WvW maps, using the same identifiers as the
 [match detail API][match-details]
* `en`, `de`, `es`, `fr`: The localized place name of the objective

This alternative can be linked against directly from [here][alternative-api] or
included as a normal JavaScript file.

Based on [this gist][gist].

[gist]: https://gist.github.com/codemasher/bac2b4f87e7af128087e
[alternative-api]: https://raw.github.com/commonquail/gw2-wvw-objectives/master/objectives.js
[objective-names]: https://api.guildwars2.com/v1/wvw/objective_names.json
[match-details]: https://api.guildwars2.com/v1/wvw/match_details.json
