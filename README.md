# JA BizTown Daily Schedule Builder

A browser-based tool for creating and printing a staff schedule for a JA BizTown simulation day. It is a standalone HTML application: there is no build step, package installation, server, or database.

## Open the app

### Run from a downloaded copy

1. Download or clone this repository.
2. Open `index.html` in a current browser such as Chrome or Edge.

The app can also be hosted as a static site. See [GitHub Pages deployment](#github-pages-deployment).

## Use the schedule builder

1. Enter the school name and mayor's name.
2. Enter the actual arrival time and confirmed departure time.
3. Leave **Break format** on **Automatic recommendation** to use one break for days under four hours and two breaks for days of four hours or more. Choose a one-break or two-break override when needed.
4. Review the schedule and any warnings. Add staff assignments in the schedule table if helpful.
5. If plans change during the day, choose the activity beginning now under **Mid-day adjustment**, enter its actual start time, and apply the revision. Completed activities stay fixed and the confirmed departure time remains the end of the schedule.
6. Select **Print / Save PDF** to print the schedule or save it as a PDF.

Confirm arrival and departure times before printing. The schedule and names are held in the open browser page; they are not saved to a server or retained after the page is closed or refreshed.

## Files

- `index.html` — the application entry point and file served by GitHub Pages.
- `ja_biztown_schedule_builder_v26.html` — a version-named copy of the same application currently in `index.html`. Keep the two files in sync if maintaining both.

## GitHub Pages deployment

No build tool or GitHub Actions workflow is required. To publish the app from this repository:

1. Open the repository's **Settings** tab.
2. In the sidebar, select **Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**, then select **Save**.
5. Wait for the Pages deployment to finish. Check the **Actions** tab for the Pages build and deployment workflow if the site does not appear.

The expected project-site address is:

<https://jani-capstone.github.io/ja-biztown-schedule-builder/>

The repository currently has no deployment workflow or Pages configuration file, and its published URL has not been verified. The address above should be treated as the expected URL until Pages is enabled and the deployment is confirmed.

## Updating the published app

Edit `index.html` and commit the change to `main`. GitHub Pages republishes the root directory after the update. If the version-named copy is kept, update it at the same time so it does not become stale.
