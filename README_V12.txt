Amsterdam House Entrances — V12

This update changes only index.html. Existing photos, entrances.geojson and
all 352 records stay untouched.

Changes:
- Geographically anchored popup follows the entrance when the map moves.
- Stable popup orientation: its anchor is chosen when opened and never flips
  automatically during map gestures.
- On opening, the map gently pans only as much as necessary to show the
  entire photo, metadata and margin. The marker stays visible beside the card.
- Popup photo is displayed without side bands or cropping. The card width
  follows the original photo aspect ratio.
- Mobile zoom buttons move to bottom-right; the typology filter remains above
  the popup in the stacking order.
- All user-interface text is in English; original addresses and type codes
  are unchanged.

Publish via GitHub Desktop:
1. Extract ZIP.
2. Replace ONLY index.html in your current repository.
3. Commit changes to main and Push origin.
4. Reload the GitHub Pages URL on a mobile device; hard refresh if cached.

Your current photos/ directory and entrances.geojson need no changes.
