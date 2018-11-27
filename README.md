# AsyncLoader
The purpose of the library is to abstract the downloading (images, pdf, zip, etc) and caching of remote resources (images, JSON, XML, etc)

# Requirements
- Use the following url for loading data: http://pastebin.com/raw/wgkJgazE
- Images and JSON should be cached efficiently (in-memory only, no need for caching to disk)
- The cache should have a configurable max capacity and should evict images not recently used
- An image load may be cancelled
- The same image may be requested by multiple sources simultaneously (even before it has loaded), and if one of the sources cancels the load, it should not affect the remaining requests
- Multiple distinct resources may be requested in parallel
- You can work under the assumption that the same URL will always return the same resource
- The library should be easy to integrate into new iOS project / apps
- You are supposed to build a solid structure and use the needed programming design patterns
- Think that the list of item returned by the API can reach 100 items or even more. At a time, you should only load 10 items, and load more from the API when the user reach the end of the list
## Requirements which may be an advantage
- Usage of size classes
- Usage of cool animations and transitions
- Adding "pull to refresh" is an advantage


