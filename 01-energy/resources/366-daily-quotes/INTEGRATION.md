# Energy Quote of the Day integration

Canonical source: energy-366-daily-quotes.csv. Derived JSON and browser module must be regenerated if the CSV changes.

Use a locally vendored copy of energy-quote.js in each static site, then call window.SLAEnergyQuotes.mount(element). For LIME 12 mount only when GICS 01 Energy is selected; call the returned cleanup function when changing sector and clear the element. Do not show energy quotes for other sectors. Calendar matching uses Asia/Kolkata and month/day, including February 29 in leap years. No daily commits required. Refreshes within 60 seconds on an open page. Preserve existing layout and CTAs. Use existing brand styles. Verify each deployment independently.

Scope: energy product tours, OmniVerse cases, 20 SuperLabs, LIME 12, energy bootcamps across enterprise domains, and daily quote components. Do not change non-energy pages.
