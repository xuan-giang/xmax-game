# SPA Xmas Game (CleverTap Popup)

## Files
- game_desktop_vi.html
- game_desktop_en.html
- game_mobile_vi.html
- game_mobile_en.html

## Assets folder
Create a folder `assets/` next to the HTML files, and put these files inside:

- sticky.png
- popup-base.png
- result-frame.png
- form-icon-1.png
- form-icon-2.png
- form-icon-3.png
- form-icon-4.png
- form-icon-5.png
- result-50.png
- result-20.png
- result-10.png
- result-8.png
- result-5.png

## Where to edit quickly
Open any HTML and find `COMMON_CONFIG`:
- Change `ASSET_BASE` if your asset path is different
- Update `COUPON_NAME_TO_RESULT_KEY` to match your real `coupon.name` values from CleverTap
- Update `PROMOTION_NAMES` if you fetch from a single promotion (set 1 item)

## Close behavior option
- `HIDE_STICKY_ON_CLOSE: false` (default) => close popup keeps sticky
- set to `true` => close popup hides sticky

## Notes
- If CleverTap is not injected, the code simulates coupon fetch for local testing.
- In CleverTap, ensure `clevertap.coupon.fetch(promoName, successCb, errorCb)` is available in your template.
