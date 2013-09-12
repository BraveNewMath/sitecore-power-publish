Sitecore Power Publish
======================

Sitecore Publish functionality improvements and extensions by Rob Habraken

This is one of the first versions of this project, it's still in progress.
Next version will also include more publish related content editor add-ons...

### Power Publish ###

First of all, this publish button will force the item being published, regardless the state of the Publishable option on the Item tab in the Publish restrictions, so you can use it to publish items that you've unpublished via the Unpublish button of this add-on (it does respect other Publishing restrictions though). But more importantly, this publish button also publishes all resources used by the current item. So if you've included media items like an image or a PDF, but forgot to publish them, clicking this button will also publish those items. It even works if you've publised the media item itself, but forgot to publish its parent folder...

This function will not publish linked pages in your site that are not published, but only resources like media library items and data sources used in item fields, as those are needed to display the item you want to publish correctly. This method even publishes the templates and layouts used by the current item, if that's not done yet.

If you are using Sitecore 7, this also works for datasource field values, as they are queryable or represented by GUIDs from version 7.0 and up. Older versions of Sitecore (6.6 and less) store datasources as plain text, hence they are not noted as reference by Sitecore and thus this plugin will not have any effect on those items.

### Unpublish ###

This button enables you to unpublish an item with a single click. It will change the Publish Restrictions as it unchecks the Publishable option on the Item tab and publishes the item after that, using a full Republish without Subitems.

## License info ##

Copyright (C) 2013 Rob Habraken

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
