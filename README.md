# Brown Original Series - Sanity CMS

This is the content management system for Brown Original Series streaming service. This CMS allows content editors to manage shows, episodes, and extras for the BOS platform.

## Accessing the CMS

The Sanity Studio is accessible at: [bos-cms.sanity.io](https://bos-cms.sanity.io)

## Content Structure

The CMS is organized into three main content types:

### Shows

Shows are the primary content unit and contain:
- **Title**: The name of the show
- **Description**: Summary of the show's content and premise
- **Hero Image**: Large banner image for the show page (16:9 aspect ratio recommended)
- **Card Image**: Thumbnail image for listings (2:3 aspect ratio recommended)
- **Credits**: Rich text field for cast, crew, and production information
- **Featured Show**: Toggle to include the show in homepage carousels
- **Slug**: Auto-generated URL-friendly identifier (based on title)

### Episodes

Episodes belong to shows and contain:
- **Title**: The episode title
- **Description**: Summary of the episode content
- **Episode Number**: Numerical order of the episode
- **Show**: Reference to the parent show
- **Mux Playback ID**: Video identifier from Mux for playback
- **Thumbnail**: Episode thumbnail image
- **Slug**: URL-friendly identifier

Episodes will appear in the CMS with the format: "Show Title Ep X: Episode Title"

### Extras

Extras are additional video content related to shows, such as behind-the-scenes, interviews, etc:
- **Title**: The extra content title
- **Description**: Summary of the extra content
- **Show**: Reference to the related show
- **Mux Playback ID**: Video identifier from Mux for playback
- **Thumbnail**: Thumbnail image
- **Slug**: URL-friendly identifier

Extras will appear in the CMS with the format: "Show Title: Extra Title"

## How to Use

### Adding a New Show

1. Navigate to "Shows" in the studio sidebar
2. Click "Create new Show"
3. Fill in all required fields (Title, Description, Hero Image, Card Image)
4. Format the Credits using the rich text editor
5. Toggle "Featured Show" if you want it to appear in the homepage carousel
6. Click "Publish" when complete

### Adding Episodes

1. Navigate to "Episodes" in the studio sidebar
2. Click "Create new Episode"
3. Fill in the Title, Description, and Episode Number
4. Select the parent Show from the dropdown
5. Add the Mux Playback ID (obtained from the video platform)
6. Upload a Thumbnail image
7. Click "Publish" when complete

### Adding Extras

1. Navigate to "Extras" in the studio sidebar
2. Click "Create new Extra"
3. Fill in the Title and Description
4. Select the related Show from the dropdown
5. Add the Mux Playback ID
6. Upload a Thumbnail image
7. Click "Publish" when complete

## Frontend URLs

The frontend will construct URLs in the following format:
- Shows: `/shows/[show-slug]`
- Episodes: `/shows/[show-slug]/[episode-slug]`
- Extras: `/shows/[show-slug]/extras/[extra-slug]`

## Need Help?

For technical assistance, contact Vincent Amato (vincent_amato@brown.edu)
