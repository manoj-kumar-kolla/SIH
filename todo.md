# Project TODO

- [x] Implement full authentication experience: login, registration, forgot password, and account management UI aligned with supported Manus OAuth.
- [x] Implement onboarding that asks for teach skills and learn skills and persists profile preferences.
- [x] Implement complementary teach/learn matching engine.
- [x] Implement browse and filter view with matched-user profile cards and ratings.
- [x] Implement skill-exchange session proposal, acceptance, and upcoming-session management.
- [x] Implement in-app notifications for matches and session state changes.
- [x] Implement post-session mutual ratings and reviews.
- [x] Implement user profile page with skills, session history, and average rating.
- [x] Apply elegant premium visual system, refined typography, responsive layout, and smooth micro-interactions.
- [x] Add Vitest coverage for matching, sessions, ratings, and authentication-adjacent behavior.
- [x] Verify browser flows, TypeScript checks, and production build.

- [x] Resolve authentication scope honestly: use supported Manus OAuth for real auth and make account management explicit, without pretending username/password fields are wired to a custom credential backend.
- [x] Fix complementary matching so a user’s teach skills match another user’s learn skills and vice versa.
- [x] Add visible accept, decline, complete, and cancel controls for upcoming skill-exchange sessions.
- [x] Create new-match notifications and surface notification read state.
- [x] Add ratings/reviews UI and enforce completed-session participant and duplicate-review guards.
- [x] Complete profile session history and average rating display.
- [x] Extend Vitest coverage for reciprocal matching, session status updates, and rating constraints.
- [x] Verify authenticated success and error flows beyond the initial screenshot.

- [x] Add calendar-based scheduling views for daily and upcoming skill-exchange sessions.
- [x] Add explicit Find matches prompts asking what the user will teach and what they will learn.
- [x] Add Discover feed for live and upcoming joinable skill-exchange sessions.
- [x] Add session join flow and participant visibility for public live sessions.
- [x] Add tests for calendar data, joinable sessions, and teach/learn filtering.
- [x] Verify the new responsive scheduling and Discover flows, then save a checkpoint.

- [x] Add Vitest coverage for live-session discovery, participant persistence, capacity limits, and calendar grouping.
- [x] Verify authenticated desktop and mobile flows for Find matches, Calendar, Discover sessions, join actions, and full-session errors.
- [x] Save a new checkpoint after the enhancement verification.

- [x] Replace the Find matches search bar with explicit teach and learn prompts connected to complementary matching.
- [x] Preserve Discover sessions without changing its current experience.
- [x] Replace the Calendar strip with a grid calendar and add-schedule flow.
- [x] Add easy profile editing for name, bio, teach skills, and learn skills.
- [x] Add tests and verify the refined desktop/mobile flows before saving a checkpoint.

- [x] Stop using saved profile teach/learn skills as the default Find matches input.
- [x] Ask fresh teach and learn questions every time Find matches is opened or reset.
- [x] Add a Process button that starts complementary session discovery and shows processing state/results.
- [x] Add tests for Process input filtering and verify the fresh-search flow before checkpoint.

- [x] Reset teach and learn prompts and processed state whenever Find matches is reopened.
- [x] Add explicit Process-flow tests for empty-input guarding and complementary results.
- [x] Re-verify fresh Find matches in the browser and save a new checkpoint.

- [x] Add a focused complementary-result test for the fresh Process search path.
- [x] Capture a new browser verification after reset-on-reopen and Process changes.
- [x] Save the final checkpoint for the fresh-search experience.

- [x] Add persistent session-specific notes with author, session, and saved timestamp.
- [x] Allow both session participants to view and save notes only within that session.
- [x] Add a personal Notes view showing only notes explicitly saved to sessions the user can access.
- [x] Add session notes editor and saved-note indicators to the Calendar/session experience.
- [x] Add tests for participant access, note saving, and personal Notes filtering.
- [x] Verify the session notes flow and save a new checkpoint.

- [x] Show a saved-note count or state badge on Calendar session rows.
- [x] Add coverage for personal Notes filtering and participant-guarded save/load behavior.
- [x] Verify the Notes UI in the browser and save the final checkpoint.

- [x] Add a repository-level participant-guard test for the session notes save/load helpers.
- [x] Save the final session-notes checkpoint after the latest UI and test changes.

- [x] Add a cute in-app helper chatbot with guidance for Find matches, Calendar, Discover sessions, My notes, and My profile.
- [x] Add a server-side helper chat procedure using the preconfigured built-in LLM without exposing credentials to the client.
- [x] Let the helper collect and validate scheduling details, then require explicit confirmation before creating a session.
- [x] Add cute chatbot face, launcher, chat panel, loading, error, and empty states.
- [x] Add tests for helper intent parsing, scheduling confirmation, and safe missing-detail handling.
- [x] Verify the helper and scheduling command flow, then save a new checkpoint.

- [x] Enforce scheduling confirmation, future time, valid partner existence, and compatible matched-user checks on the server.
- [x] Add explicit chatbot empty states for incomplete details, no draft, and no compatible matched user.
- [x] Add tests for assistant response intent parsing, missing fields, and the scheduling mutation safety path.
- [x] Verify the Pippa conversation and confirmed scheduling flow in the browser, then save a new checkpoint.

- [x] Add an explicit server-side partner existence check in the Pippa scheduling mutation.
- [x] Add distinct chatbot states for no draft, incomplete details, and no compatible matched user.
- [x] Add direct tests for assistant scheduling guards including confirmation, past time, incompatible partner, and missing partner.
- [x] Verify an end-to-end Pippa scheduling conversation and save the final checkpoint.

- [x] Upgrade visible branding from Symbiosis to SkillSwap with the requested tagline and clearer exchange concept.
- [x] Refine entry/auth copy and CTA hierarchy without changing supported authentication behavior.
- [x] Add dashboard summary cards for best matches, teaching, learning, upcoming sessions, rating, and completed exchanges using real data only.
- [x] Improve match cards with clearer match percentage, teach/learn reciprocity, rating, completed exchanges, and Connect/View profile actions where supported.
- [x] Improve Calendar/session presentation with clearer upcoming/completed/cancelled grouping and status treatments.
- [x] Add a polished light/dark/system theme toggle and ensure the design tokens adapt across the app.
- [x] Improve responsive navigation, empty/loading/error states, accessibility, and consistent design tokens.
- [x] Add tests and responsive visual verification for the product polish upgrade, then save a new checkpoint.

- [x] Finish the SkillSwap rebrand with the exact tagline and a clearer teach/learn exchange demonstration.
- [x] Add a real completed-exchanges summary card from session data.
- [x] Add reciprocal match labels, completed-exchange metadata, and a View profile action where supported.
- [x] Group Calendar sessions into Upcoming, Completed, and Cancelled sections with clear status treatments.
- [x] Extend ThemeContext and UI to support Light, Dark, and System modes.
- [x] Complete accessible responsive navigation, focus states, loading/error/empty states, and polish-focused tests.
- [x] Verify the polish changes and save a new checkpoint.

- [x] Add a clear reciprocal exchange demo to the SkillSwap entry experience using explicit teach/learn framing.
- [x] Add real completed-session counts to match cards from available session data.
- [x] Refactor Calendar into distinct Upcoming, Completed, and Cancelled sections while preserving existing actions.
- [x] Replace the theme cycle button with a visible Light, Dark, and System selector showing the active mode.
- [x] Add visible focus states and consistent major-screen loading, error, and empty states.
- [x] Add tests for theme selection and grouped-session rendering data, then save a new checkpoint.

- [x] Refactor Calendar into real Upcoming, Completed, and Cancelled sections while preserving all existing session actions.
- [x] Add explicit visible focus styles and consistent major-screen state treatments.
- [x] Add a grouped-session UI contract test and verify the grouped Calendar at desktop and mobile widths.
- [x] Save the final product-polish checkpoint.

- [x] Add a focused SessionGroups contract test covering section labels and preserved action categories.
- [x] Review and refine major-screen loading, error, and empty states without claiming unsupported behavior.
- [x] Capture final desktop and mobile previews after the SessionGroups refactor.
- [x] Save a new checkpoint after final verification.

- [x] Add consistent loading, error, and empty states for Find matches, Calendar, Notes, Notifications, and Profile.
- [x] Verify the state treatments with the final build and previews.
- [x] Save a new checkpoint after the final SkillSwap polish changes.

- [x] Add shared loading and error states for My notes and Notifications.
- [x] Capture fresh desktop and mobile previews after the final state-treatment edits.
- [x] Save a new checkpoint after the final verified SkillSwap polish changes.

- [x] Capture a fresh desktop preview after the final Notes and Notifications state-treatment edits.
- [x] Save a new checkpoint after the final verified SkillSwap polish changes.

- [x] Review the latest GridCalendar edit against the requested visual intent.
- [x] Remove invalid inline opacity 10 overrides and preserve the calendar’s existing visual hierarchy.
- [x] Run TypeScript, tests, production build, and calendar preview verification.
- [x] Save a new checkpoint after the corrected calendar edit.

- [x] Capture a fresh preview after removing the invalid GridCalendar opacity overrides.
- [x] Save a new checkpoint after the corrected GridCalendar edit and final verification.

- [x] Brighten the Calendar schedule dialog with an opaque white surface, stronger border/shadow, and high-contrast inputs and CTA.
- [x] Verify the dialog styling and save a new checkpoint.

- [x] Refine schedule-dialog inputs with opaque white surfaces, dark text, bright focus rings, and clear borders.
- [x] Refine the primary Add to calendar CTA with a brighter accent and strong contrast.
- [x] Capture a visual preview with the schedule dialog open.
- [x] Save a new checkpoint after the verified schedule-dialog update.

- [x] Verify the bright opaque schedule dialog itself in an open-dialog preview or equivalent focused visual check.
- [x] Save a new checkpoint after the final schedule-dialog refinements.

- [x] Add a post-login area selector shown before the main SkillSwap dashboard on each login.
- [x] Render Find matches, Discover sessions, Calendar, My notes, and My profile as vertical cards on a horizontal oval carousel.
- [x] Support sideways scrolling/dragging and make the centered card visually prominent.
- [x] Allow clicking the centered or any visible card to enter the corresponding main-site area.
- [x] Add a clear skip/back affordance without bypassing the required area-selection experience unintentionally.
- [x] Add tests and verify desktop/mobile carousel behavior, then save a new checkpoint.

- [x] Make clicking any visible area card enter that SkillSwap area directly while preserving center emphasis for scrolling.
- [x] Add an explicit back/close affordance that returns to the authenticated dashboard without bypassing the first-login selector requirement by default.
- [x] Add focused selector logic tests for card mapping, direct entry, and centered-state behavior.
- [x] Re-run checks and desktop/mobile verification, then save a new checkpoint.

- [x] Make the return-to-dashboard affordance a temporary dismissal that does not persistently bypass the selector on the next login.
- [x] Add deterministic helpers and tests for direct-entry selection and centered-card state.
- [x] Re-run checks and desktop/mobile previews after the final selector correction.
- [x] Save a new checkpoint after the final selector verification.

- [x] Replace the full-screen overlay feel with an integrated dashboard navigation layer that keeps the SkillSwap shell visible.
- [x] Make the selected area transition directly into the existing main content while preserving sidebar and topbar context.
- [x] Add a clear integrated back/area-switch action instead of treating the selector as a separate widget.
- [x] Refine desktop/mobile composition, focus states, and transitions for the integrated selector.
- [x] Add tests and verify the integrated navigation flow before saving a new checkpoint.

- [x] Add a persistent Area switcher action inside the dashboard so users can reopen the integrated selector after entering a section.
- [x] Add explicit focus-visible styles and transition states for selector cards, close control, and area switcher.
- [x] Add an integrated-flow contract test covering open selector, choose area, return to dashboard, and reopen behavior.
- [x] Re-run TypeScript, tests, production build, and desktop/mobile previews, then save a new checkpoint.

- [x] Add direct open, choose, close, and reopen selector-flow helpers and tests.
- [x] Save a new checkpoint after the final integrated-selector verification.

- [x] Remove the post-login oval area selector and its related selector-only flow.
- [x] Redesign the phone experience as a dedicated mobile layout instead of a condensed desktop dashboard.
- [x] Add mobile-specific navigation, spacing, hierarchy, and touch-friendly interaction treatments while preserving desktop behavior.
- [x] Verify the updated desktop and mobile flows with tests, build checks, and responsive previews, then save a checkpoint.

- [x] Adapt SkillSwap’s visual system to the provided PeerLearn reference without changing functionality.
- [x] Restyle desktop and mobile surfaces with the reference’s airy cool palette, centered orbit accents, elevated white cards, and restrained borders.
- [x] Brighten Pippa’s launcher, panel, messages, confirmation state, and controls across desktop and mobile.
- [x] Verify unchanged behavior with tests, production build, and responsive visual previews, then save a checkpoint.

- [x] Make the top profile avatar a keyboard-accessible shortcut to My profile on every click.
- [x] Add a clear logout button in the account/profile area while preserving the existing logout behavior.
- [x] Verify the profile shortcut and logout flow at desktop and mobile widths, then save a checkpoint.

- [x] Remove unintended broad padding styles injected by the visual editor while retaining the intended banner copy and orbit adjustment.
- [x] Verify the banner copy remains unobscured and save the corrected visual-editor checkpoint.

- [x] Redesign only the mobile login page as a dedicated phone-first composition instead of a condensed desktop split layout.
- [x] Preserve desktop login layout and existing authentication actions.
- [x] Verify mobile login at phone width plus desktop/auth build checks, then save a checkpoint.

- [x] Capture an explicit unauthenticated mobile login preview for the dedicated phone-first layout.
- [x] Save a new checkpoint after the verified mobile-login redesign.

- [x] Move the Best matches, Teaching, Learning, Upcoming, Completed, and Rating summary cards below the main Find matches task area.
- [x] Preserve the existing summary data, matching inputs, Process action, and responsive behavior.
- [x] Verify the reordered Find matches page at desktop and mobile widths, then save a checkpoint.

- [x] Capture explicit authenticated desktop and mobile previews showing summary cards below the Find matches area.
- [x] Save a new checkpoint after the verified Find matches layout reorder.

- [x] Preserve the attached pasted_content_2.txt brief in the project as a reference document without changing application functionality.
- [x] Save a checkpoint that includes the preserved brief for recovery.

- [x] Preserve pasted_content_3.txt as a project reference brief without applying its visual recommendations.
- [x] Save a checkpoint that includes the newly preserved visual-polish brief.

- [x] Preserve pasted_content_4.txt as a project reference brief without applying its background recommendations.
- [x] Save a checkpoint that includes the newly preserved background-design brief.

- [x] Add a coherent SkillSwap motif system using teach/learn arrows, exchange lines, skill doodles, nodes, and abstract connection shapes.
- [x] Add tasteful animated background layers to the dashboard and login page without obscuring content or changing functionality.
- [x] Add responsive reductions and prefers-reduced-motion safeguards for all decorative animation.
- [x] Verify desktop, tablet, mobile, dark mode, readability, accessibility, tests, and build, then save a checkpoint.

- [x] Simplify the abstract background decoration into a cleaner, more intentional visual treatment after the failed editor target.
- [x] Verify the revised decoration does not obscure content or change functionality, then save a checkpoint.

- [x] Adapt the dashboard and login background toward the provided indigo-violet/cyan luminous skill-network reference.
- [x] Add connected skill nodes, orbit paths, soft glow fields, and a central teach/learn exchange motif without making text unreadable.
- [x] Add responsive and reduced-motion safeguards while preserving all existing functionality.
- [x] Verify desktop/mobile/login readability, tests, build, and save a checkpoint.

- [x] Redesign the login screen with the supplied lavender learning-exchange composition and SkillSwap brand treatment.
- [x] Preserve the existing login, create-account, forgot-password, and Manus sign-in behavior without adding unsupported providers.
- [x] Add responsive desktop/mobile login styling, readable contrast, and accessible controls matching the new composition.
- [x] Verify the login screen with tests, build, browser previews, then save a checkpoint.

- [x] Use the supplied login image unchanged as the visual login surface.
- [x] Preserve the existing functional login, create-account, forgot-password, and Manus sign-in controls without modifying the image.
- [x] Verify exact asset usage, responsive behavior, auth controls, tests, build, and save a checkpoint.

- [x] Preserve pasted_content_5.txt as a focused login redesign reference without applying its recommendations.
- [x] Save a checkpoint that includes the newly preserved login redesign brief.

- [x] Replace fragile transparent login hotspots with reliable functional controls over the unchanged supplied artwork.
- [x] Make login controls visible to assistive technology and keyboard-accessible while preserving the current auth handlers.
- [x] Verify Log in, Create account, Forgot password, Continue securely, and Manus sign-in at desktop/mobile widths, then save a checkpoint.

- [x] Add a reliable functional hotspot for the embedded Create an account button in the unchanged supplied artwork.

- [x] Remove the visual editor’s unintended nested paddingBottom injection from AuthView and child elements.
- [x] Preserve only the intended AuthView bottom spacing if it remains visually useful.
- [x] Verify the unchanged login image and functional auth controls, then save a checkpoint.

- [x] Reduce the condensed feel of the exact-image login by improving auth-card width, padding, field spacing, and action hierarchy.
- [x] Preserve the supplied artwork unchanged and keep all auth controls functional and keyboard-accessible.
- [x] Verify desktop and mobile login composition, tests, build, and save a checkpoint.

- [x] Replace the exact supplied login image treatment with an original recreation inspired by its lavender learning-exchange language.
- [x] Remove exact-image framing and fragile image-only hotspot positioning while keeping functional auth controls.
- [x] Rebuild responsive original motifs, verify login interactions and readability, then save a checkpoint.

- [x] Tune the original login recreation toward the attached airy glass-card reference with soft animated orbs and floating exchange cards.
- [x] Refine the hero headline, gradient emphasis, spacing, and auth-card hierarchy without copying the source markup or changing auth behavior.
- [x] Verify desktop/mobile responsiveness, reduced motion, auth controls, tests, build, and save a checkpoint.

- [x] Redesign the mobile login as a dedicated phone-first composition with generous spacing instead of a condensed desktop stack.
- [x] Keep the desktop login unchanged and preserve all existing auth controls and handlers.
- [x] Verify mobile readability, touch targets, auth interactions, tests, build, and save a checkpoint.

- [x] Simplify the mobile login hero so it uses less vertical space and does not compete with the form.
- [x] Enlarge and space the mobile auth card and controls so the login flow feels deliberate and comfortable.
- [x] Verify the second mobile pass at the actual phone viewport, preserve desktop behavior, and save a checkpoint.

- [x] Rework only the mobile login into a spacious phone-first composition instead of a condensed desktop-derived layout.
- [x] Preserve the laptop login layout, exact desktop selectors, and existing auth handlers.
- [x] Verify phone readability, touch targets, desktop preservation, tests, build, and save a checkpoint.

- [x] Remove the visual editor’s broad inline `color: #ffffff` injection from AuthView and nested controls.
- [x] Preserve the intended targeted text color only where it improves the visual treatment.
- [x] Verify login readability, auth interactions, tests, build, and save a checkpoint.

- [x] Consolidate the login styles into one intentional responsive system instead of layered breakpoint overrides.
- [x] Make the laptop and mobile login compositions both spacious, balanced, and visually coherent.
- [x] Preserve all auth controls and verify laptop/mobile previews, tests, build, and save a checkpoint.

- [x] Add a small accessible close button in the top-right of Pippa’s open chat panel.
- [x] Wire the close button to the existing Pippa panel state without changing chat or scheduling behavior.
- [x] Verify close behavior at desktop and mobile widths, then save a checkpoint.

- [x] Brighten low-contrast dashboard and login text treatments after the failed visual-editor target.
- [x] Preserve layout, functionality, theme behavior, and control states while improving readability.
- [x] Verify contrast at desktop/mobile and light/dark states, then save a checkpoint.

- [x] Improve the mobile login composition with clearer hero-to-form spacing, larger readable text, and comfortable touch controls.
- [x] Brighten remaining low-contrast mobile text across login, dashboard, cards, navigation, and Pippa surfaces.
- [x] Preserve the laptop layout and functionality, verify phone/laptop previews, tests, build, and save a checkpoint.

- [x] Brighten green and black text that remains low-contrast across mobile and shared SkillSwap surfaces without changing layout or functionality.
- [x] Verify the brighter text at mobile and desktop widths, then save a checkpoint.

- [x] Make all login text use normal, high-contrast colors so it is clearly visible on the login surface.
- [x] Brighten or recolor low-contrast site text across shared dashboard surfaces without changing layout or functionality.
- [x] Verify login and site readability at mobile and desktop widths, then save a checkpoint.

- [x] Brighten and recolor the listed Find matches, Discover, Calendar, Profile, Notes, and Session history headings and empty-state copy.
- [x] Verify all listed surfaces at mobile and desktop widths, then save a checkpoint.

- [x] Brighten the remaining listed Discover, Calendar, session-status, Notes, and Profile text on its actual card backgrounds.
- [x] Verify the remaining listed surfaces at mobile and desktop widths, then save a checkpoint.

- [x] Enforce black text on white surfaces and white text on dark surfaces for every user-listed item.
- [x] Verify all listed text at mobile and desktop widths, then save a checkpoint.

- [x] Make A little nudge, SCHEDULE, August 2026, YOUR PROFILE, and Manoj Kumar text black.
- [x] Verify the requested black labels and save a checkpoint.

- [x] Review the failed LiveDiscover visual edit and manually make the targeted text black if it was not applied.
- [x] Verify the LiveDiscover correction and save a checkpoint.

- [x] Restore the original text styling by removing the recent contrast overrides and reverting the manual LiveDiscover text edit.
- [x] Verify the restored styling at mobile and desktop widths, then save a rollback checkpoint.

- [x] Make only the four specified My Profile session-history texts visible with isolated styles.
- [x] Verify the profile-only text fix at mobile and desktop widths, then save a checkpoint.

- [x] Review the three failed Home.tsx comment-based white-text edits and locate their intended profile targets.
- [x] Verify any isolated white-text correction at mobile and desktop widths, then save a checkpoint.

- [x] Review the failed LiveDiscover white-heading and condensed-layout comments.
- [x] Apply a targeted white hero heading and improve Discover spacing without changing functionality.
- [x] Verify LiveDiscover at mobile and desktop widths, then save a checkpoint.

- [x] Review the failed LiveDiscover heading white-text edit and confirm the isolated heading rule.
- [x] Verify the LiveDiscover heading treatment and save a checkpoint.

- [x] Recheck the repeated failed LiveDiscover white-heading edit and confirm the existing isolated rule.
- [x] Verify the heading treatment and save a checkpoint without unnecessary changes.

- [x] Make the LiveDiscover hero heading visibly change against its actual rendered background.
- [x] Verify the visible change at mobile and desktop widths, then save a checkpoint.

- [x] Make only “Choose your next room.” white in LiveDiscover.
- [x] Verify the isolated heading edit and save a checkpoint.

- [x] Review the failed SessionGroups and Home white-text comments and identify the exact targets.
- [x] Apply isolated white text to the intended elements, verify, and save a checkpoint.

- [x] Review the six failed Home b/p/span white-text comments and identify the exact targets.
- [x] Apply isolated white text to those Home targets, verify, and save a checkpoint.

- [x] Make the exact recently edited Home text visibly white with direct isolated selectors.
- [x] Verify the visible Home text result and save a checkpoint.

- [x] Review the latest Home.tsx visual-editor color edits and remove unintended global inline color propagation.
- [x] Preserve the five intended Home text color changes through isolated selectors without changing layout or functionality.
- [x] Verify TypeScript, tests, production build, and responsive previews, then save a checkpoint.

- [x] Identify the Home element behind the failed comment and compare it with Discover Sessions styling.
- [x] Apply the intended Discover Sessions-inspired visual treatment through isolated selectors without changing functionality.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Identify the stale Home and SessionGroups visual-comment targets and review their current presentation.
- [x] Apply focused visual polish to the identified Home and SessionGroups elements without changing functionality.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Review shared layout and page styling surfaces behind the failed app-wide Home visual comment.
- [x] Apply consistent visual polish across the main pages without changing functionality.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Review the latest Home visual-editor change and remove unintended global black inline propagation.
- [x] Restore the surrounding dashboard to its original appearance while preserving only the requested targeted text edit.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Restore the mistakenly changed Home styling to its prior state.
- [x] Apply only the selected Home element’s intended visual edit.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Review the latest Home visual-editor propagation and identify the selected bold element.
- [x] Remove propagated black styles and apply the Discover Sessions-inspired treatment only to the selected bold element.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Identify the stale Home target and compare it with the Discover Sessions reference styling.
- [x] Apply the matching treatment only to the identified Home element without broad propagation.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Review the latest GridCalendar and SessionGroups editor propagation and identify the selected elements.
- [x] Remove propagated styles and apply only the selected calendar and session text color changes.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Review the ProfileEditor visual-editor propagation and identify the selected Save changes button.
- [x] Remove propagated styles and apply only the selected Save changes button color.
- [x] Verify TypeScript, tests, production build, responsive previews, and save a checkpoint.

- [x] Confirm the ProfileEditor Save changes color edit is persisted in the current project state.
- [x] Re-verify and save a confirmed checkpoint if the edit is missing or unsaved.

- [x] Review the latest ProfileEditor propagation and identify the selected Save changes button.
- [x] Remove propagated #09090c styles and preserve only the selected button edit.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Identify the stale ProfileEditor div target and compare its surface with Discover Sessions.
- [x] Apply the matching Discover Sessions treatment only to the identified ProfileEditor surface.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Identify the stale Home div target and compare it with the Discover Sessions reference.
- [x] Apply the matching Discover Sessions treatment only to the identified Home surface.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Review the latest Home visual comment and identify the stale target.
- [x] Apply focused Home polish only to the intended surface if it is not already implemented.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Identify the exact Home sidebar note containing “Small steps, shared.” and “Every session is a chance to grow together.”.
- [x] Apply the requested isolated visual edit only to that sidebar note.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Review the latest Home background-color propagation and identify the selected bold element.
- [x] Remove propagated #dcc6c6 styles and preserve only the selected bold-element background color.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

- [x] Review the latest ProfileEditor light-text propagation and identify the selected paragraph.
- [x] Remove propagated #fafcff styles and preserve only the selected paragraph color.
- [x] Verify TypeScript, tests, production build, and save a checkpoint.

## SkillSwap collaboration expansion

- [x] Keep Light mode unchanged and add a separate inverted Dark-mode token layer.
- [x] Extend reciprocal user/session data with experience, session type, availability, language, and capacity fields.
- [x] Calculate and display explainable compatibility percentages on learner cards.
- [x] Show the current user’s teach/learn session details as a simple rounded rectangular learner card after processing Find Matches.
- [x] Add Discover topic search and filters for skill, rating, experience, availability, duration, level, language, online-only, and role.
- [x] Preserve teacher/learner role switching per session rather than permanently assigning roles.
- [x] Add one-to-one capacity controls with a data model ready for small groups and workshops.
- [x] Add protected in-app messaging for matched users before sessions.
- [x] Add a protected meeting workspace with camera/microphone/leave controls, participant list, chat, screen sharing, whiteboard, text/code editor, optional file sharing, and report/block controls.
- [x] Add private session notes and file upload/download authorization for participants.
- [x] Add report/block procedures and minimize exposed personal data in all cards, Discover results, chat, and meeting views.
- [x] Add schema migrations, server procedures, Vitest coverage, responsive verification, and staged checkpoints for the collaboration expansion.

## Learner-card visibility fix

- [x] Trace why filled teach/learn prompts do not render the current learner card.
- [x] Add an editable learner-card flow for private/public visibility, session time, and participant capacity.
- [x] Ensure Discover renders available online learner cards and preserves privacy-safe data.
- [x] Add tests, responsive verification, and save a checkpoint.

## ResizeObserver warning fix

- [x] Trace the recurring ResizeObserver loop warning to its dashboard/layout source.
- [x] Apply the smallest safe fix without changing intended layout behavior.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## ResizeObserver follow-up

- [x] Trace why the existing ResizeObserver diagnostic guard is not preventing the reported browser error.
- [x] Harden the narrowly scoped ResizeObserver handling without masking unrelated runtime errors.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## Home removal request

- [x] Resolve the stale Home-section target by confirming the user’s exact requested removal was the Discover learner-card empty-state message.
- [x] Preserve the Home layout and adjacent functionality while removing only the clarified Discover learner-card empty-state message.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint for the clarified removal.

## Discover empty-state removal

- [x] Remove only the message “No other learner cards match yet. Your card is ready above. Publish it publicly to let people discover your exchange.”.
- [x] Preserve the learner card, publishing controls, Discover results, and other dashboard functionality.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## MyLearnerCard visibility edit

- [x] Inspect the failed visual-edit target at MyLearnerCard.tsx:17 and identify the intended invisible content.
- [x] Apply only the necessary visibility correction without changing learner-card behavior or unrelated styling.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## MyLearnerCard condensed-layout edit

- [x] Inspect the failed visual-edit target at MyLearnerCard.tsx:17 and identify the condensed layout constraints.
- [x] Apply only a responsive spacing and layout correction that makes the learner card less condensed without changing behavior.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## MyLearnerCard repeated condensed-layout edit

- [x] Inspect the current MyLearnerCard structure and rendered constraints at the stale target.
- [x] Apply a stronger responsive layout correction so the card is clearly less condensed without changing behavior.
- [x] Run TypeScript, tests, production build, multi-breakpoint browser verification, and save a checkpoint.

## LiveDiscover removal request

- [x] Resolve the stale LiveDiscover.tsx:27 target by confirming the user’s exact requested removal was the live-room empty-state copy.
- [x] Preserve live-session discovery and join behavior while removing only the clarified empty-state copy.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint for the clarified removal.

## Live Discover empty-state removal

- [x] Remove only the message “No live rooms match those filters. Try a broader topic, level, language, or duration.”.
- [x] Preserve live-room discovery, filters, learner cards, and Join session controls.
- [x] Run TypeScript, tests, production build, browser verification, and save a checkpoint.

## Discover Sessions and Discover People navigation

- [x] Inspect current navigation, active-area state, and existing LiveDiscover/LearnerCard data flow.
- [x] Add a dedicated Discover Sessions area that lists all available learner cards.
- [x] Rename the existing live-session area and navigation labels to Discover People without changing its live-room behavior.
- [x] Update desktop/mobile navigation, headings, and accessible labels consistently.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Discover People live-only refinement

- [x] Inspect the current Discover People composition and identify learner-card content rendered there.
- [x] Keep Discover People limited to live-session discovery while keeping all learner cards on Discover Sessions.
- [x] Preserve live-session search, filters, and Join session behavior.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Restore Discover People and refine Discover Sessions

- [x] Compare the current LiveDiscover and DiscoverSessions components with the last correct Discover People checkpoint.
- [x] Restore Discover People to the intended live-session discovery experience.
- [x] Apply the learner-card discovery treatment to Discover Sessions without removing its dedicated learner-card purpose.
- [x] Preserve navigation, filters, Join session behavior, matching, and privacy-safe data handling.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a corrective checkpoint.

## Discover Sessions live-only refinement

- [x] Inspect current Discover Sessions and Discover People content ownership.
- [x] Make Discover Sessions show only live sessions by reusing the established live-session discovery experience.
- [x] Keep the learner-card experience in Discover People unchanged.
- [x] Preserve live-session search, filters, Join session behavior, privacy-safe data, and responsive navigation.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Empty visual-edit verification

- [x] Inspect the current project state and confirm no visual-edit changes were supplied.
- [x] Verify Discover Sessions remains live-session-only and Discover People remains intact.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Second empty visual-edit verification

- [x] Inspect the current source and confirm no visual-edit changes were supplied.
- [x] Re-verify Discover Sessions remains live-session-only and Discover People remains intact.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Move Find Matches inputs into learner card

- [x] Inspect the current Find Matches prompt state and MyLearnerCard props/state flow.
- [x] Remove the separate teach and learn input bars from Find Matches.
- [x] Add editable teach and learn inputs inside MyLearnerCard and keep Process/search behavior working.
- [x] Preserve Publish to Discover as the action that makes the card publicly discoverable.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Keep one learner-card action

- [x] Remove the duplicate Process action from MyLearnerCard.
- [x] Keep one Publish to Discover action at the bottom-left of the card.
- [x] Preserve teach/learn inputs, public discovery publishing, private-session behavior, and responsive layout.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Fix learner-card future-time validation

- [x] Inspect the datetime-local default and publish validation in MyLearnerCard.
- [x] Remove the future-time requirement while retaining valid datetime parsing.
- [x] Continue rejecting malformed session times.
- [x] Run TypeScript, tests, production build, responsive browser verification, and save a checkpoint.

## Public and private learner-card access

- [x] Remove the future-time requirement from learner-card publishing.
- [x] Make public learner cards visible to everyone in Discover.
- [x] Generate a six-digit access code for private sessions.
- [x] Restrict private-session joining to users with the matching code or owner access.
- [x] Show private access details to the owner and preserve privacy-safe card rendering.
- [x] Run schema/API/UI tests, TypeScript, production build, responsive verification, and save a checkpoint.

## Replace summaries with live learner card

- [x] Remove the Best Matches, Teaching, Learning, Upcoming, Completed, and Rating summary strip.
- [x] Show the user’s active published learner card in that area.
- [x] Add an edit control that reopens the learner-card fields.
- [x] Add a cancel-session control that cancels the overall published session safely.
- [x] Preserve public/private visibility, private access-code protection, and Discover behavior.
- [x] Run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Reuse duplicate hosted sessions

- [x] Inspect the active-session lookup and publish flow.
- [x] Reuse the user’s existing active session when teach and learn values match.
- [x] Update the existing session’s settings instead of inserting a duplicate.
- [x] Allow different topics or previously cancelled sessions to create new sessions.
- [x] Add regression coverage and run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Host admission for published sessions

- [x] Inspect session participants, meeting access, and current join flow.
- [x] Add join-request persistence and host-only admit/deny procedures.
- [x] Make non-admitted users wait instead of entering the meeting workspace.
- [x] Add a host popup listing requests with Admit and Deny controls.
- [x] Connect admitted users to the existing Zoom-like meeting workspace.
- [x] Preserve private access-code restrictions and participant capacity.
- [x] Add regression coverage and run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Restore Discover People visibility

- [x] Inspect why learner cards are missing from Discover People.
- [x] Restore the previous visible learner-card behavior without weakening public/private access rules.
- [x] Preserve live-session discovery, join requests, and host admission controls.
- [x] Add regression coverage and run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Trace Discover People visibility again

- [x] Trace the active navigation path, showLearners prop, query response, and empty-state conditions.
- [x] Fix the concrete issue preventing learner cards from appearing by returning all privacy-safe user profiles, including profiles still in progress.
- [x] Preserve live sessions, join requests, and host admission behavior.
- [x] Run TypeScript, tests, production build, responsive verification, and save a corrective checkpoint.

## Learner-card admission popup and Start flow

- [x] Inspect the current request block, admission polling, and MeetingWorkspace opener.
- [x] Replace the request block with a learner-card popup showing requester details and Admit/Deny controls.
- [x] Show an explicit Start button after admission and open the existing video conference workspace only when Start is clicked.
- [x] Preserve private access-code checks, participant limits, host authorization, and privacy-safe requester data.
- [x] Add regression coverage and run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## MyLearnerCard visibility polish

- [x] Inspect the stale line 133 target and identify the invisible learner-card area.
- [x] Apply a narrow contrast, spacing, or surface fix only to that area.
- [x] Preserve popup, admission, Start, publishing, editing, and cancellation behavior.
- [x] Run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Fix self-participant mutation error

- [x] Trace which participant action is sending the current user as the selected participant.
- [x] Prevent the current user from appearing as an eligible participant and return a clear safe state.
- [x] Preserve valid participant selection, hosting, and meeting behavior.
- [x] Add regression coverage and run TypeScript, tests, production build, responsive verification, and save a checkpoint.

## Repair conference start, chat, and admission return

- [x] Trace why Start video conference currently only activates the local camera instead of connecting the meeting workspace.
- [x] Trace why in-session chat cannot deliver messages and identify the correct participant target for hosts and admitted joiners.
- [x] Implement a real browser peer-connection flow with signaling and clear fallback states for unavailable media or peer support.
- [x] Make in-session chat reliably address the other admitted participant and preserve self-participant protection.
- [x] After host admission, return the host to the active learner/session card with admitted-participant status and a Start conference action.
- [x] Add regression coverage for conference signaling, chat targeting, and post-admission navigation.
- [x] Run TypeScript, Vitest, production build, responsive browser verification, and save a checkpoint.

## End live sessions cleanly and retain completed history

- [x] Trace how MeetingWorkspace closes, how live Discover Sessions are queried, and how completed sessions appear in Profile history.
- [x] Add an explicit End session action that marks the session completed for authorized participants and releases it from live discovery.
- [x] Ensure Discover Sessions returns only active live rooms and excludes completed, cancelled, and declined sessions.
- [x] Preserve completed sessions in Profile history with a clear completed state and any saved session notes.
- [x] Add regression coverage for end-session authorization, discovery filtering, and profile-history retention.
- [x] Run TypeScript, Vitest, production build, responsive verification, and save a checkpoint.

## Professional publish, conference pop-out, and abandoned-session cleanup

- [x] Save the current working state as a checkpoint named “almost” before making new changes.
- [x] Make Publish to Discover open a clear host waiting-room popup with all join requests and Admit/Deny controls.
- [x] Keep an explicit Conference action available after admission and open the meeting in a professional expandable/minimizable pop-out surface.
- [x] Treat public sessions with zero joined participants as abandoned after 24 hours without updates and remove them from active discovery without deleting valid history.
- [x] Add regression coverage for waiting-room visibility, pop-out controls, 24-hour abandonment, and retained completed history.
- [x] Run TypeScript, Vitest, production build, responsive verification, and save the final checkpoint.

## Expand conference pop-out by default

- [x] Open the conference pop-out in its expanded state by default.
- [x] Make the expanded state fill the available screen cleanly and keep the minimize control reversible.
- [x] Verify desktop and mobile layouts, then run tests and save a checkpoint.

## Ratings, visible waiting states, and out-of-session messages

- [x] Trace completed-session rating state, queue/waiting messages, Join Interest behavior, and current messaging procedures.
- [x] Prompt both participants after session completion to rate the exchange and optionally leave a comment, without duplicating submitted ratings.
- [x] Make queue, waiting-room, admission, and unavailable-session messages visually prominent in light and dark themes.
- [x] Make Join Interest open the selected person’s privacy-safe profile with available sessions, ratings, and a message action.
- [x] Add a Messages navigation item and inbox view for conversations outside sessions, preserving self-participant protection.
- [x] Add regression coverage and run TypeScript, Vitest, production build, responsive verification, and save a checkpoint.

## Verify stale Home visual edit

- [x] Review the failed Home.tsx visual-edit target and confirm whether the intended text visibility is already correct.
- [x] Apply only a scoped visibility fix if the intended target is still not visible; otherwise preserve the current styling.
- [x] Run TypeScript, tests, production build, preview verification, and save a checkpoint.

## Fix meeting file upload and shared whiteboard

- [x] Trace the browser upload payload, upload mutation validation, storage helper, and meeting file display.
- [x] Normalize browser file uploads into an accepted payload with safe size/type validation and clear errors.
- [x] Trace whiteboard state writes and reads for both admitted participants.
- [x] Synchronize whiteboard snapshots through protected meeting state so the other participant sees updates and late joiners receive the latest canvas.
- [x] Add regression coverage and run TypeScript, Vitest, production build, responsive meeting verification, and save a checkpoint.

## Private session code access

- [ ] Trace private code generation, host learner-card data, and Discover Sessions join handling.
- [ ] Show the active private session’s six-digit access code clearly on the host learner card with copy support.
- [ ] Add a prominent six-digit code-entry bar above Discover Sessions cards and route valid codes into the existing private join flow.
- [ ] Preserve privacy, host admission, and invalid-code error handling.
- [ ] Add regression coverage, run TypeScript, Vitest, production build, responsive verification, and save a checkpoint.
