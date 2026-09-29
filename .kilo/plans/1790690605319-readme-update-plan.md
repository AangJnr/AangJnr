# Plan to Update README.md with Current Project Information and Screenshots

## Objective
Update README.md to reflect current project information from PROJECT_INFO.md and new screenshot locations in `resources/app_screenshots/`. Create per-project README files for projects with >5 screenshots.

## Project Inventory

### Projects from PROJECT_INFO.md (11 projects)
1. **Endow Payments** (2 entries - payment links + full platform)
2. **DependrScoots** - Scooter rental app
3. **Smart Advertisement Platform** - Smart ad platform
4. **Robot Control Queuing System** - Smart Clean
5. **Regardless** - Sports/fitness platform
6. **Jambl Beats App** - Music creation
7. **Echo Client Feedback App** - Feedback platform
8. **Wine2U** - Wine delivery

### Screenshot Folders Available (13 folders)
- cloop/ - 6 screenshots (Cloopp/Recycle Box)
- contena/ - 10 screenshots (Contena Logistics)
- endow/ - 13 files (5 images, 4 videos, 4 mobile/web variants)
- finddance/ - 9 screenshots
- jambl/ - 4 screenshots
- regardless_app/ - 12 screenshots + app_store_listings/
- scoots/ - 27 screenshots + 2 videos + mockup folders
- smart_clean/ - 2 screenshots
- smartly/ - 15 screenshots + 1 video
- station_locator/ - 10 screenshots
- wholesome_craft/ - 5 screenshots
- wine2U/ - 6 screenshots + 1 video

## Mapping Projects to Folders
| Project (PROJECT_INFO.md) | Screenshot Folder | Screenshot Count |
|---------------------------|-------------------|------------------|
| Contena Logistics | contena/ | 10 |
| Find.Dance | finddance/ | 9 |
| Cloopp (Recycle Box) | cloop/ | 6 |
| Smart Advertisement Platform | smartly/ | 16 |
| Robot Control Queuing System | smart_clean/ | 2 |
| DependrScoots | scoots/ | 29 |
| Regardless | regardless_app/ | 12 + app store |
| Jambl Beats App | jambl/ | 4 |
| Echo Client Feedback | (no folder) | 0 |
| Endow Payments | endow/ | 13 |
| Wine2U | wine2U/ | 7 |
| Wholesome Craft | wholesome_craft/ | 5 |
| Station Locator | station_locator/ | 10 |

Note: Some projects in PROJECT_INFO.md don't have matching screenshot folders (Echo). Some folders don't have matching PROJECT_INFO entries (station_locator, wholesome_craft, cloop).

## Implementation Plan

### Phase 1: Update Main README.md
1. **Preserve header** (bio, contact info, tech stack badges)
2. **Reorganize Projects section** with current projects from PROJECT_INFO.md
3. **For each project with screenshots:**
   - Use project description from PROJECT_INFO.md
   - Show 2-3 screenshots in main README (mix of mobile/web as appropriate)
   - For projects with >5 screenshots: add link to per-project README
   - Use new paths: `resources/app_screenshots/<folder>/<image>`
4. **Image layout rules:**
   - Portrait/mobile: 3 columns max
   - Landscape/web: 1-2 columns
   - Mixed: 2-3 images per project
   - Videos: embed if available (GitHub supports mp4)

### Phase 2: Create Per-Project READMEs (for projects with >5 screenshots)
Create `resources/app_screenshots/<folder>/README.md` for:
- contena/ (10)
- endow/ (13)
- finddance/ (9)
- regardless_app/ (12 + app store)
- scoots/ (29)
- smartly/ (16)
- station_locator/ (10)
- wine2U/ (7)

Each per-project README includes:
- Project title and brief description
- All screenshots with captions
- Videos embedded
- App store listings (for regardless_app)

### Phase 3: Handle Special Cases
- **regardless_app**: Use app_store_listings/ subfolder, prioritize those preserving numbering
- **scoots**: Include both screenshots and videos (dependr_scoots_dashboard.mp4, dependr_scoots_mvp.mp4)
- **smartly**: Include create_ad.mp4 video
- **wine2U**: Include rwgjgg9yhru83op0skip.mp4 video
- **endow**: Include mobile and desktop videos

## Tasks

1. [ ] Parse PROJECT_INFO.md for structured project data
2. [ ] Generate updated main README.md content
3. [ ] Create per-project README.md files in each screenshot folder
4. [ ] Update image paths from old locations to new `resources/app_screenshots/` paths
5. [ ] Handle video embedding in markdown
6. [ ] Verify all referenced images exist

## Output
- Updated `README.md` at repo root
- Per-project README.md files in `resources/app_screenshots/<folder>/`

## Validation
- All image paths resolve to existing files
- No broken links
- Consistent formatting across projects
- Mobile/portrait images displayed in 3-column layout
- Landscape/web images displayed in 1-2 column layout