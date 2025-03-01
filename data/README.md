# Videos Data

This JSON file contains all the videos and categories for the Salaf Feed application.

## How to Add or Edit Videos

To add a new video or edit an existing one, simply modify the `videos.json` file in this directory.

### Adding a New Video

Add a new object to the `videos` array with the following structure:

```json
{
  "id": "10",  // Use a unique ID
  "title": "Your Video Title",
  "thumbnail": "https://example.com/thumbnail.jpg",  // URL to the thumbnail image
  "embedId": "YouTubeVideoID",  // The YouTube video ID from the URL
  "category": "Category Name",  // Must match one of the existing categories
  "views": "0",  // Formatted view count
  "likes": "0",  // Formatted like count
  "uploadedAt": "Just now"  // Formatted upload time
}
```

### Adding a New Category

Add a new object to the `categories` array with the following structure:

```json
{
  "id": "7",  // Use a unique ID
  "name": "Category Name",  // The display name of the category
  "icon": ""  // Optional icon (currently not used)
}
```

### Editing Existing Content

Simply find the video or category you want to edit in the JSON file and modify its properties.

## Notes

- The `id` field must be unique for each video and category
- The `category` field in videos must match the `name` field of one of the categories
- Thumbnail URLs should be direct links to images
- YouTube embed IDs are the part of the YouTube URL after `v=` (e.g., for `https://www.youtube.com/watch?v=dQw4w9WgXcQ`, the embed ID is `dQw4w9WgXcQ`)