[< Back](../../README.md#sections)

# @TODOs

### High Priority

- [ ] **`gui & api`:** Complete the implementation of the supported exchanges
- [ ] ...

### Medium Priority

- [ ] **`api`:** Create a benchmarking system to improve the database’s performance
- [ ] ...

### Low Priority

- [ ] **`gui`:** Allow users to toggle between `light` and `dark` mode
- [ ] **`gui`:** Make the users' list searchable
- [ ] **`gui & api`:** Make the Blacklisted IP addresses searchable
- [ ] **`gui`:** Create Bitcoin Quotes Component and place it in `sign-in` and `update-password`
- [ ] **`api`:** Store server metrics (usage%, load%, temperature°) in OHLC format
- [ ] **`api`:** Expand the automated tests' coverage
- [ ] **`gui`:** Fix the glitch in `mobile-tabs.component.tsx` that makes the tabs lag ~1 second before placing themselves correctly (this issue may be caused by the `min-h-dvh` class set in the parent container)
- [ ] **`gui`:** Create a component that can render any data element (including JSX elements) and can be passed to the `info-dialog` and `confirmation-dialog` components
- [ ] **`gui`:** Fix responsiveness issues with long texts and apply the solution in:
  - `Server/Monitoring`, `Server/APIErrors`, `Server/APIErrorDialog`, `APIError` badges
  - `Adjustments`
  - `Users/AuthSessions`
  - `IPBlacklist`(IP & notes)
  - `NotificationsDialog` (`SenderBadge`)
  - Version Card in: `MainSidenav`, `PlatformUpdate`, `Server/Monitoring`
- [ ] **`gui`:** Fix weird glitch in the `coins-state-dialog` and `liquidity-state-dialog` components that closes the dialog without a trace when the viewport is resized. If `lightweight-charts` is causing this, consider using a different library for this components
- [ ] **`gui`:** Improve `app-installer`, make the content clickable and add a close button like the toastr
- [ ] **`api`:** Create `record-list-store` module and reduce code duplication by leveraging the power of object composition. Also evaluate if the `canRecordsBeListed` function should be exposed too. Finally, implement it on:
  - `api-error`
  - `ip-blacklist`
  - `notification`
  - ...
- [ ] **`gui`:** Enable users to query custom date ranges in the `positions` component
- [ ] ...
